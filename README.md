
# DoorDash Payment System Analysis Report

<div style="text-align: center;">
    <img src="https://lh7-us.googleusercontent.com/ziZbvdZQErvyVnPbqk7Nv9kZ7gIBFg56XbVKZ0PD_pQuOUUVSBZpbdw2tgr2MU1ZBC-hUIZuzvsXg9DPyE1BE5xDT_pLJBONYBjhrkVtOI08cxTblamw_wdQHNBYBteNyIRqcjdZK-hehTc0shImBpc" width="400" height="200" />
</div>

## 🚀 Overview

This README summarizes the comprehensive analysis of DoorDash's payment system, highlighting key frameworks, security considerations, and recommendations for maintaining a secure and efficient payment infrastructure. Our goal is to ensure DoorDash's system is robust against security threats while offering a seamless user experience.

## 🗝️ Key Findings

### Payment System Overview

- DoorDash employs payment gateways like Stripe and Visa Direct for customer transactions.
- Security is paramount, with encryption and compliance frameworks such as PCI-DSS in place to protect customer information.
[Details]
- Doordash payment system involves multiple steps and various components starting from the customer till the payment is completed
    
- Doordash utilizes payment gateways such as Stripe and Visa Direct for handling payments from customers
    
- Point of Sale (PoS) are used in abundance and forms an important part of the payment system
    
- DoorDash's payment system is designed to be simple and practical for consumers and businesses, while also providing fair compensation for Dashers
<img src="https://lh7-us.googleusercontent.com/1DchhscDCV54Pq9-J39RnHFRfONqm0ksyhKeC_MqouTv-g64G5SSgiNOeMzSm1YNtLMHxfm8wxvDOQfXcb4GxFyYL-lDEhs13BhA4Ujh9UqLSu9GIpiwqX3cu8IElekxVo6-rEBSF57dIj5GxAUsdg=s2048" width="400" height="300" />

### Security Challenges

- Historical breaches in 2019 and 2022 highlight vulnerabilities in third-party components, underscoring the need for continuous security enhancement.
[Details]
- All of the payment gateways and the Doordash software has to be secure against attacks by regularly staying compliant with set frameworks and testing procedures
- PII of customers has to be secured at every phase of payment and should use proper encryption mechanisms
- Security breach could result in putting a hold to Doordash’s operations
- The hack of 2019 and 2022 showed how a potential third part vulnerability can result in compromising CVVs, credit card number, names & other sensitive info about the customers
- The security aspect of the system must be constantly updated on all possible attack vectors.
### Framework Analysis

- **PCI-DSS**: Essential for payment data compliance, offering a structured approach to security but requiring significant effort and resources.
- **STRIDE**: Provides a comprehensive model for identifying threats, although it can be resource-intensive.
- **PASTA**: A risk-centric framework that emphasizes the identification and mitigation of security risks.
- **OCTAVE FORTE**: Focuses on risk management, offering a detailed understanding of potential system risks.
- **NIST CSF**: Advocates for a balanced cybersecurity posture across five core functions: Identify, Protect, Detect, Respond, and Recover.
- **No Framework**: Suggests a more customized approach to security, focusing on specific DoorDash needs but lacking the structured guidance of established frameworks.

## Detailed Framework Analysis Report

### PCI-DSS
DoorDash, as a payment processor and a merchant, is required to comply with the Payment Card Industry Data Security Standard. PCI-DSS, Payment Card Industry Data Security Standard, defines a set of security standards to protect cardholders’ data and prevent fraud. Every merchant dealing with payment must comply with the 12 requirements defined under PCI-DSS. Failure to comply with the same can result in penalties, fines & legal actions. Ever since DoorDash suffered data breaches, especially some data loss-related credit cards, there has been a major opportunity to reevaluate the overall security posture in the payment department. Thus, we must analyze the PCI-DSS framework on the current structure to the compliance of the same

<img src="https://lh7-us.googleusercontent.com/suuruNOtYbXM2TDXKsMfqAA5Zx4QsAuiXfpfjhsYiv8hUn0Xe14zwcMYbeuXuqoq5JT_0GX5csTce50e9H28vfX3TIrG0ap_IhS4BsXOp5TvQBZAeIwCFfOhp-eMRScYyp4teHSIYBpXBITg5-NJXw=s2048" width="300" height="300" />


**Metric of Success**
A high percentage of successful audits would suggest that DoorDash is successfully putting in place and maintaining the appropriate security controls, as well as that it is taking the necessary precautions to safeguard its payment systems and customer data against data breaches and cyberattacks. A successful audit could serve to increase client confidence and give businesses a competitive edge [4].

### STRIDE 
This framework was developed by two engineers from Microsoft in the 1990’s. The six components of STRIDE framework are spoofing, tampering, repudiation, information disclosure, denial of service, and elevation of privilege. [5]
Payment systems such as one DoorDash are vulnerable to multiple attacks which are well documented based on past incidents on payment systems. Attackers are always finding ways to attack these systems since the benefits of such an attack are huge for an attacker. An attacker who successfully manages to exploit a component within the network that handles these transactions, the transfer of data from the Point of Sale to the bank databases, or any component that is involved in the payment would have a huge benefit-to-risk ratio.


<img src="https://lh7-us.googleusercontent.com/xQSyNGdpOmxNjPtzNbsDWw7USpmEbvI787xoD09JVz0mE_5gmjiNKcATqN1FVA4aZLpw9C8ic_3R4TZP9QRNFLPwuV1LmZBJXxNA-YOKvYsm3ch9EKsMjQUY5ty8PFAx0slihFfZrQK_pLZyJSbQv2g" width="300" height="300" />



**Advantages:**
- With the STRIDE framework, the focus is more on the risks associated with any system. Payment systems require careful analysis of all kinds of potential risks associated with them through various components in the entire payment flow starting from the customer’s device to the server and the payment gateways. [13]
- Another major advantage is that Doordash could use STRIDE and other threat modeling frameworks to analyze potential threats since STRIDE is compatible with other frameworks. 
**Disadvantages:**
- It could take a lot of time and resources to identify all of the threats in Doordash’s payment system since it is complex and involves third-party payment gateways as well. When a new feature has to be introduced, analyzing threats using STRIDE could take away a lot of useful time that could be used in the development of the new feature which would help the company. [14]
- It requires expertise to efficiently utilize the STRIDE framework to analyze threats because analysis at a high level may be easy but to back any proposals for change with evidence is a challenge that is faced by inexperienced individuals in the field.

**Metric of Success**
If the threats from external devices and internal systems are minimal in the report after STRIDE analysis, it would mean that DoorDash has implemented required security controls to secure data. If STRIDE analysis is done regularly and with careful analysis and discussions, it would be possible to eliminate chances of new attacks or zero days as well since it checks the systems in depth and covers non-overlapping areas.

### PASTA
It is a risk-centric threat modeling, PASTA framework provides a comprehensive, risk-centric approach to identifying and managing risks associated with the payment system, it can help DoorDash ensure the security and efficiency of the payment system, which is crucial to its success.
DoorDash is very careful about protecting its payment system. If any security lapse occurs, it could lead to a lot of money being lost and DoorDash's reputation being damaged. So, DoorDash has put together a very strict security system to deal with any potential problems.


<img src="https://lh7-us.googleusercontent.com/5vxb_W6_w2slh9iuoqBLYo_XKtWJhnHtjDeZWAPyzlG3spnE_PY9DCCxQlRpkIM57T8WcEI69suBdOptqxmBQ7882XQwamtxXBJZUUEovW5Q6MecNZRcP25OfIdNfyLeZwUmPtNhmHZ2A4oKhaLnng8" width="400" height="300" />


**PASTA Implementation**

- **Business Objective:** The purpose of this plan is to protect DoorDash's payment system from any possible security risks, and make sure our company is following industry standards and regulations.
- **Technical Scope:** To protect DoorDash's payment system from potential data breaches, unauthorized access, and phishing attacks, the company has implemented a variety of security protocols and systems.
- **App Decomposition:** We will investigate DoorDash's payment system to see if there are any weaknesses or risks. We will then put in place security processes, such as two-factor authentication, end-to-end encryption, and frequent vulnerability testing.
- **Threat Analysis:** The analysis of threats involves examining all possible ways in which they can occur and devising strategies to prevent their occurrence. No information regarding the threat analysis can be left out in the paraphrasing process.
- **Vulnerability Detection:** Our strategy involves implementing security measures to monitor and identify potential risks to the payment system. Prompt remedial action will be taken upon detection of any issues.
- **Attack Enumeration:** We will have a plan of action in place in the case of a security breach to act immediately and limit the harm.
- **Risk/Impact Analysis:** Our focus will be on assessing the potential financial and reputational consequences associated with a security breach, and implementing measures to mitigate them.
**Advantages:**
This proposal offers several benefits, such as strengthening DoorDash's payment system security, ensuring compliance with industry regulations and standards, and enhancing customer trust and satisfaction. No information has been left out in this paraphrased text.
**Disadvantages:**
The cost and possible disturbance to the payment system are the primary drawbacks of putting a security framework into action. Additionally, it demands continuous maintenance and observation.
**Metrics for Success:**
For a company to achieve success, it is crucial to avoid any security breaches, adhere to the industry's standards and regulations, enhance customer trust and satisfaction, and generate a profitable return on investment. No information can be left out for a company to prosper

### OCTAVE FORTE
OCTAVE FORTE is a comprehensive risk management framework that can be used to identify, assess, and prioritize risks related to DoorDash's payment system. It is crucial to ensure the security of the payment system to prevent data breaches, fraudulent transactions, data corruption, and various other cyberattacks. This framework can help identify the several security risks to the system and potential mitigation measures. It can ultimately help DoorDash in safeguarding its payment system and ensuring the confidentiality, integrity, and availability of its customers' sensitive information.


<img src="https://lh7-us.googleusercontent.com/oBnjhTc5Rb_-HXRLr76BcdshnbQ9fm3WZSHOsh8umGevsUZkINyRKQDsZPx7Qa8Be7Dit2e5G5Q_RuqKS2G6WGqtTtiu-2fMtCIUEk4oeswZWNVqTEZzYKYRfb2jl3ru52kzRGA-n7PYr8afn08K66Y" width="400" height="200" />


**Details**

1. Establish Risk Governance and Appetite:  
We need to first establish a governance structure that provides direction regarding the assigned roles and responsibilities, policies to be followed, resources needed, and information flow within the organization [1]. The following is the level of risk that DoorDash is willing to accept in relation to its payment gateway:
- Huge revenue loss associated with payment gateway downtime 
- Loss of customer trust following a data breach of customer information
- Failure to achieve security compliance can damage DoorDash’s reputation and prevent future business partnerships.
1. Scope Critical Services & Assets:  
We must identify and prioritize the critical services and assets related to our payment gateway. This involves identifying the information assets, systems, and applications that are critical to the operation of the payment gateway. Our critical services and assets are:
- Payment System
- Customer Data 
1. Identify Resilience Requirements of Assets:  
The resilience requirements of our payment gateway assets must be identified to ensure they are adequately protected against potential risks. The following is the criticality of our assets and the impact of potential disruptions:
- Payment System: Requires high availability to ensure that transactions can be processed quickly and securely, along with strong data confidentiality to protect the sensitive financial information of its users. 
- Customer Data: A data breach can lead to the leaking of customer data and payment details. Security measures should be kept in place to ensure the confidentiality of this data. Furthermore, data redundancy and backups can ensure availability in the event of a system failure or data loss.
4. Measure Current Capabilities:  
The current controls and policies implemented to secure these assets are the following:

- Firewalls and intrusion detection/prevention systems are in place to protect against unauthorized access and malicious traffic.
- Data encryption protects sensitive payment information during transit and at rest.
- Monitor for any unauthorized access or activities related to customer data.
- Regular security testing to identify any potential vulnerabilities in the payment system and address them promptly.
- Patch servers and payment software regularly.  
5. Identify Risks, Threats, and Vulnerabilities to Assets

|   |   |   |   |   |   |
|---|---|---|---|---|---|
||Asset|Actor|Motive|Access|Outcome|
|Ransomware|Customer Data|APT|Monetary gain|Payment system servers|Financial loss|
|Data Corruption|Customer Data|Malicious competitor|Disrupt business operations|Payment Database|Financial loss|
|DoS/DDoS|Payment Gateway|APT or Hacktivists|Disrupt business operations|Payment Gateway|Operational downtime and financial loss|
|Data Breach|Customer Data|APT or state-sponsored actors|Monetary gain|Payment Database|Reputational damage, Legal and regulatory penalties|

6. Analyze Risks Against Capabilities:  
Our current security capabilities fall short of the aforementioned threats.
- There is currently a lack of authentication at the payment gateway that allows for leaked financial information to be used for fraudulent transactions. 
- Our firewall rules are not configured to deal with a sudden influx in large volumes of traffic. This leaves our network and payment gateway vulnerable to DoS attacks.
- The lack of regular data backups leaves us susceptible to huge financial losses in the event of a ransomware attack or data corruption.
7. Plan for Response: 
- Multi-factor authentication should be put in place to ensure that only authorized individuals can access sensitive information or systems.
- Taking regular data backups can help mitigate ransomware and data corruption threats.
- Traffic filtering and appropriate rate-limiting should be implemented at firewalls to mitigate the risk of DoS attacks. 
- Load balancers can help distribute large volumes of traffic reaching the payment gateway and ensure high availability.
- Regularly update action plans to align with our risk appetite and prioritize the security of our most critical assets.
8. Implement the Response Plan:
- Assign responsibilities and roles for implementing the response plan and ensure necessary resources are allocated.
- Develop and implement policies and procedures for secure access and usage of payment gateway and customer data systems.
- Train employees and stakeholders on the new policies and procedures and ensure compliance with the new security measures.
- Regularly review and monitor the effectiveness of the implemented response plan and security controls.
- Continuously update and improve the response plan and security measures to align with the evolving threat landscape and the company's risk appetite.
**Advantage**
- Provides detailed understanding of the risks associated with current payment system
- Helps determine the specific areas that require improvement.
- Structured approach 
**Disadvantage**
- Resource-intensive and requires a lot of effort. 
- A very time-consuming process
**Metrics for Success:**
- DoorDash develops a thorough response to identified risks 
- Prioritize security investments based on organization's risk appetite
- Effective implementation of controls can enhance payment system security 
### NIST CSF
NIST CSF can help DoorDash reduce the risk of data corruption by identifying important data assets and setting up suitable protections to prevent corruption.
NIST CSF can help Doordash as to
- reduce the risk of zero-day attacks on its payment mechanisms by implementing a risk-based vulnerability management program
- address the prevalent risk of DoS attacks by enforcing the implementation of controls such as network segmentation, intrusion prevention systems, and incident response plans for DoS incidents.
- points out the need for response to data breaches by identifying critical data assets (especially payment information), implementing appropriate safeguards to protect against unauthorized access, confidentiality of payment mechanisms and establishing incident response plans for data breaches, etc.


<img src="https://lh7-us.googleusercontent.com/I9VqZCPm2QnpGmKxZtSmOE8pWuWxP-bU4cf692UabpXc95oOS8Q3y3YdOwq1v6JMF5h3wsiRKDdk2UJZXUKlIznwF0AJQ0BpfcWjj_XPOx6jbDOyOmNyoTE65GnIYdK0pWySZ1zK-OkKbKPiTiRPz3k" width="400" height="200" />

**Why NIST CSF is good for Doordash?**
1. Data corruption on Payment Database: By identifying important data assets and setting up suitable protections to prevent corruption, the NIST CSF can assist Doordash in reducing the risk of data corruption. The framework can be used to set up procedures for keeping an eye out for spotting instances of data corruption. 
2. Social engineering: The NIST CSF can help organizations address the risk of social engineering attacks by implementing controls such as security awareness training for employees, multi-factor authentication, and access controls. The framework can also be used to establish incident response plans for social engineering scenarios.
3. Zero-day attacks on payment processing mechanisms: The NIST CSF can help Doordash to reduce the risk of zero-day attacks on its payment mechanisms by implementing a risk-based vulnerability management program, which emphasizes the inclusion of regular vulnerability scanning and patching. It also highlights the importance of continuous monitoring for the detection of potential zero-day exploits.
4. Denial-of-Service (DoS) attacks on payment gateways: The NIST CSF can help Doordash address prevalent the risk of DoS attacks by enforcing the implementation of controls such as network segmentation, intrusion prevention systems, and incident response plans for DoS incidents. DoorDash is a very dynamic platform and undergoing a Dos attack to its payment gateways might become fatal to business and can challenge its sustenance. 
5. Data breach from users payment-information database: As a client-centric company, reputation drives the business of Doordash. NIST CSF also points out the need for response to data breaches by identifying critical data assets (especially payment information), implementing appropriate safeguards to protect against unauthorized access, confidentiality of payment mechanisms and establishing incident response plans for data breaches, etc. 
**Advantage of using NIST CSF**
- NIST CSF emphasizes continuous improvement, which the organization can benefit a lot from. Doordash will be constantly on the loop for improved security enhancements towards emerging threats in a changing business environment especially on its payment systems.
- The flexibility of NIST CSF makes it easier for adoption. 
- NIST CSF is popular in the industry and implementing it is indeed a recognition for Doordash.
- Comprehensive Approach - The NIST CSF integrates numerous cybersecurity domains, such as identify, protect, detect, respond, and recover, toward its approach to cybersecurity risk management. DoorDash uses this strategy to make sure that every facet of their cybersecurity program is taken care of. The payment mechanisms will be resilient against a wide range of cyber attacks if NIST CSF is effectively implemented.
**Disadvantage of using NIST CSF**
- Complexity - Organizations with little access to cybersecurity resources and experience may find it challenging to execute the NIST CSF. More time and upfront costs may be required as a result.
- Resource-Intensive - The NIST CSF implementation process can be time-consuming, resource-intensive, and expensive. To successfully execute the framework, organizations might need to make investments towards hiring additional cybersecurity employees, equipment, and more training for effective implementation.
- Even if NIST CSF is considered as a very versatile and customizable framework, it is hard and time consuming for the framework to be aptly customized for a specific requirement. 
- Minimal Instructions on Incident Response- Although the NIST CSF offers instructions on developing an incident response plan, it does not include particular instructions on how to handle incidents on payment mechanisms.To make sure that it is ready to respond to these kind of threats and situations, DoorDash may need to adopt extra incident response rules and processes.
**Metric of success for NIST CSF**
DoorDash could track a number of variables to assess how well their cybersecurity program has improved to protect its payment processing by using the NIST CSF. Reducing cybersecurity risk is one of the framework's main objectives, thus DoorDash might assess performance by monitoring changes in its risk profile over time. DoorDash can also measure the success of the framework by tracking its ability to detect, contain, and respond to cybersecurity incidents, as well as employee participation in cybersecurity training programs. Finally, implementing the NIST CSF can help organizations reduce the cost of cybersecurity incidents and improve the efficiency of their cybersecurity programs, so DoorDash can track cost savings related to cybersecurity incidents and efficiency gains from implementing standardized policies and procedures.  

### Recommendations

- Implementing a combination of PCI-DSS and NIST CSF frameworks can offer comprehensive protection and compliance.
- Continuous monitoring and updating of security practices are crucial for mitigating emerging threats.

## 🛡️ Security Enhancements

- Regular audits and compliance checks are recommended to ensure adherence to security standards.
- Investment in security awareness training for staff to prevent social engineering and phishing attacks.

## 📈 Planning & Timeline

A detailed timeline for implementing security enhancements, including budget considerations, has been provided to guide DoorDash through the process effectively.

## 🎯 Success Metrics

- Reduction in security incidents.
- Successful compliance audits.
- Enhanced customer trust and satisfaction.

## 🤖 Technology and Tools

Emphasis on using encryption for data in transit and at rest, regular system checks, and risk management strategies to ensure the integrity and confidentiality of payment data.

## 🔍 Conclusion

DoorDash's commitment to security and efficient payment processing is evident through its compliance with key frameworks and proactive security measures. By adhering to recommended practices, DoorDash can continue to protect its customers and maintain its reputation as a secure and reliable food delivery service.

---

## Reference
1. Payment Card Industry Security Standards Council. (2021). PCI Data Security Standards (PCI DSS). https://www.pcisecuritystandards.org/pci-security-standards/
2. Foster, R., & Laberis, B. (2016). The cost of PCI DSS compliance: A framework for estimating the cost of meeting PCI DSS requirements. Journal of Information Systems Applied Research, 9(3), 22-31. Retrieved from https://journals.tdl.org/jisar/article/view/7689/6861
3. American Institute of Certified Public Accountants (AICPA). (2019). Payment Card Industry Data Security Standard (PCI DSS) Compliance: An Implementation Guide. Retrieved from https://www.aicpa.org/content/dam/aicpa/research/standards/paymentcardindustrystandards/downloadabledocuments/pci-dss-implementation-guide.pdf
4. Ismail, N., & Ali, N. A. M. (2016). A critical analysis of PCI DSS implementation: Benefits, challenges and recommendations. Journal of Theoretical and Applied Information Technology, 85(2), 224-233.
5. Hewko, A. (2023). STRIDE Threat Modeling: What You Need to Know. Software Secured. https://www.softwaresecured.com/stride-threat-modeling/
6. A02 Cryptographic Failures - OWASP Top 10:2021. (n.d.). https://owasp.org/Top10/A02_2021-Cryptographic_Failures/
7. OWASP Top Ten | OWASP Foundation. (n.d.-b). https://owasp.org/www-project-top-ten/
8. Awati, R. (2021). nonrepudiation. Security. https://www.techtarget.com/searchsecurity/definition/nonrepudiation

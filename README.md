
# DoorDash Payment System Analysis Report
**![](https://lh7-us.googleusercontent.com/ziZbvdZQErvyVnPbqk7Nv9kZ7gIBFg56XbVKZ0PD_pQuOUUVSBZpbdw2tgr2MU1ZBC-hUIZuzvsXg9DPyE1BE5xDT_pLJBONYBjhrkVtOI08cxTblamw_wdQHNBYBteNyIRqcjdZK-hehTc0shImBpc)**

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
-**![](https://lh7-us.googleusercontent.com/1DchhscDCV54Pq9-J39RnHFRfONqm0ksyhKeC_MqouTv-g64G5SSgiNOeMzSm1YNtLMHxfm8wxvDOQfXcb4GxFyYL-lDEhs13BhA4Ujh9UqLSu9GIpiwqX3cu8IElekxVo6-rEBSF57dIj5GxAUsdg=s2048)**
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

**![](https://lh7-us.googleusercontent.com/suuruNOtYbXM2TDXKsMfqAA5Zx4QsAuiXfpfjhsYiv8hUn0Xe14zwcMYbeuXuqoq5JT_0GX5csTce50e9H28vfX3TIrG0ap_IhS4BsXOp5TvQBZAeIwCFfOhp-eMRScYyp4teHSIYBpXBITg5-NJXw=s2048)**

**

|                                                        |                                                                                                                                                                      |                                                                                                         |                                                            |
| ------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------- |
| Process                                                | Detail                                                                                                                                                               | Budget                                                                                                  | Timeline                                                   |
| Identify the project's scope, set goals and objectives | outline the necessary procedures to achieve PCI-DSS compliance in the first month of the project                                                                     | $ 20,000<br><br>(Allocate resources to help define the scope)                                           | May 1 to May 30, 2023                                      |
| Perform vulnerability scans and assessment             | Perform vulnerability scans and evaluate the security posture of the systems and procedures involved in payment processing during the second month.                  | $200,000<br><br>(Cost of vulnerability scanning tools and consulting fees for vulnerability assessment) | June 1 to June 30, 2023                                    |
| Remediation and upgrades                               | Address any vulnerabilities found and carry out the appropriate system and process improvements to bring them in line with PCI-DSS requirements.                     | $250,000<br><br>(Depending on the specific remediation and upgrade requirements)                        | July 1 to August 1, 2023<br><br>(Additional buffer 7 days) |
| Data encryption and network segmentation               | Implement data encryption and network segmentation strategies to safeguard sensitive data and thwart unauthorized access.                                            | $50,000<br><br>(Cost for data encryption and network segmentation)                                      | August 8 to August 30, 2023                                |
| Testing and audit preparation                          | Perform testing to guarantee that processes and systems are operating as intended and in conformity with PCI-DSS requirements. In advance of the audit, become ready | $30,000<br><br>(Resources for testing and preparing for the audit)                                      | September 1 to October 15, 2023                            |
| Audit and compliance certification                     | If all requirements are completed, you will pass an audit conducted by a certified security assessor.                                                                | $60,000<br><br>(Cost for the external auditor and any remediation costs necessary after the audit)      | October 15 to October 30, 2023                             |
| Total                                                  |                                                                                                                                                                      | Cost - $610,000                                                                                         | Time - 6 months                                            |



**

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

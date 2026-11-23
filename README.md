# aws-iam-grc-risk-assessment
This project is phase 2 of my AWS IAM RBAC project. In this GRC project I assessed the IAM security risk, evaluated controls and documented remediation actions.

AWS IAM Security Risk Assessment

# Project Overview

I assessed three IAM controls (RBAC,least privilege, and MFA) against the NIST SP 800-53 Access Control and Identification and Authentication families. 
  - RBAC: Effective. Every user gets permissions through a department based IAM group.
  - Least Privilege: Effective for the actions tested. Unauthorized S3 uploads and IAM admin actions were denied. A full permission review is still needed.
  - MFA: Partially validated. MFA is confirmed for privileged admin account only. The other users have not been verified yet.

Three risks were identified and each rated moderate(12/25). Two remediation actions are tracked in a POA&M. 

Deliverable                                                             
------------
1. Risk Assessment Report Link: [AWS.Risk_Assessment_Report (3).pdf](https://github.com/user-attachments/files/35286795/AWS.Risk_Assessment_Report.3.pdf)

2. Risk Assessment Workbook Link: [AWS-IAM-Risk-Assessment (1).xlsx](https://github.com/user-attachments/files/35286806/AWS-IAM-Risk-Assessment.1.xlsx)

Description
-------------
1. Risk Assessment Report: Full written report- scope, methodology, results, remediation, and limitation.
2. Risk Assessment Workbook: Risk register, evidence log, findings & gap assessment, POA&M, and a heat map.



# Project Objectives
- Identify potential security risks related to AWS IAM.
- Evaluate existing access controls and permissions.
- Assess risk based on likelihood and potential business impact.
- Map relevant security controls to NIST SP 800-53 framework.
- Document remediation recommendations and track outstanding risks.

# Environment
The assessment builds on a simulates A environment containing department based user access, including IT, Finance, Sales, Marketing and HR. IAM users, groups and policies are used to examine how to access permissions align with job responsibilities.

# Scope
The initial assessment focuses on: 
- Lease Privilege and excessive permissions
- Multi-factor authentication
- User and group access management
- Access to Amazon S3 resources
- Security control documentation and remediation planning

# Methodology 
1. Identify assets and potential security risks.
2. Review existing IAM configurations and available evidence.
3. Assess risk likelihood and impact.
4. Identify relevant NIST SP 800-53 security controls.
5. Recommend remediation actions and document findings.

# Project Deliverables 
- Risk Register
- Security Control Assessment
- Risk Remediation Plan (POA&M)

# Results 

| Finding | Control | Result | Gap |
|---|---|---|---|
| F-001 | Role-Based Access Control |  Effective | None identified in testing |
| F-002 | Least Privilege |  Effective for tested actions | No comprehensive permission review; custom S3 policy resource scope needs validation |
| F-003 | Multi-Factor Authentication |  Partially validated | MFA confirmed for John.Admin only; remaining users not verified |






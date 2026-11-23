# aws-iam-grc-risk-assessment

# A hands on governance, risk & compliance assessment of identity and access controls in a simulated AWS environment, using NIST SP 800-53. 

  **Background:** This project is phase two of my AWS IAM RBAC project. In this GRC project I assessed the IAM security risk, evaluated controls and documented remediation actions.

# Project Overview

I assessed three IAM controls (RBAC, least privilege, and MFA) against the NIST SP 800-53 Access Control and Identification and Authentication families. 
  - **RBAC:** Effective. Every user gets permissions through a department based IAM group.
  - **Least Privilege:** Effective for the actions tested. Unauthorized S3 uploads and IAM admin actions were denied. A full permission review is still needed.
  - **MFA:** Partially validated. MFA is confirmed for privileged admin account only. The other users have not been verified yet.

Three risks were identified and each rated moderate(12/25). Two remediation actions are tracked in a POA&M. 

# Deliverable                                                             

1. **Risk Assessment Report Link:** [AWS.Risk_Assessment_Report (3).pdf](https://github.com/user-attachments/files/35286795/AWS.Risk_Assessment_Report.3.pdf)

2. **Risk Assessment Workbook Link:** [AWS-IAM-Risk-Assessment (1).xlsx](https://github.com/user-attachments/files/35286806/AWS-IAM-Risk-Assessment.1.xlsx)

Description
-------------
1. **Risk Assessment Report:** Full written report- scope, methodology, results, remediation, and limitation.
2. **Risk Assessment Workbook:** Risk register, evidence log, findings & gap assessment, POA&M, and a heat map.

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
1. **Review:** inventoried IAM users, groups and attached policies.
2. **Test:** signed in as each user and recorded which actions succeeded or were denied.
3. **Document evidence:** logged 17 evidence items (E-001 – E-017) with the related risk and control.
4. **Gap assessment:** compared each control against its assessment criteria (Effective / Partially Validated / Not Effective).
5. **Score risk:** Likelihood (1–5) × Impact (1–5), giving Low 1–4, Moderate 5–14, High 15–25.
6. **Plan remediation:** recorded each corrective action in a Plan of Action & Milestones (POA&M) with an owner, target date and the evidence needed to close it.

**NIST SP 800-53 controls referenced:** AC-2 Account Management · AC-3 Access Enforcement · AC-6 Least Privilege · IA-2 Identification & Authentication · AU-2 Event Logging (R-003, future work)
# Results 

| Finding | Control | Result | Gap |
|---|---|---|---|
| F-001 | Role-Based Access Control |  Effective | None identified in testing |
| F-002 | Least Privilege |  Effective for tested actions | No comprehensive permission review; custom S3 policy resource scope needs validation |
| F-003 | Multi-Factor Authentication |  Partially validated | MFA confirmed for John.Admin only; remaining users not verified |

# Remediation plan (POA&M)
| ID | Finding | Action | Priority | Target | Status |
|---|---|---|---|---|---|
| PA-001 | F-002 / R-001 | Review all IAM policies and group permissions; validate the custom S3 policy's resource scope; restrict access to job requirements | Moderate | Dec 20, 2026 |  Open |
| PA-002 | F-003 / R-002 | Verify MFA enrollment for all users; enable MFA where missing; require MFA for privileged accounts | Moderate | Dec 16, 2026 |  Open |




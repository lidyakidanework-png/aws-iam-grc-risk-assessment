#AWS IAM Security Control Assessment

#Purpose 

This document records the review of selected security controls within a simulated AWS environment. The objective is to determine whether existing IAM configurations support appropriate access management and risk reduction. 

#Assessment Status
Initial planning - control testing and evidence collection have not yet been completed. 

# Control 1: Access Enforcement
- **Control Objective:** Ensure users can access only the resources and functions authorized for their roles. 
- **Framework Reference:** NIST SP 800-53 AC-3 - Access Enforcement.
- **Assessment Procedure:** Review IAM group memberships, attached policies, and effective permissions. Test whether users can access resources outside their intended responsibilities.
-  **Evidence Required:** IAM policy configurations, group memberships, and documented access text results.
-  **Result:** Not yet assessed.
-  **Findings:** Pending evidence collection.
-  **Recommended Action:** Correct excessive permissions and validate that access restrictions work as intended.

# Control 2: Account Management
- **Control Objective:** Ensure user accounts and their permissions are managed appropriately. 
- **Framework Reference:** NIST SP 800-53 AC-2 - Account Management.
- **Assessment Procedure:** Review the simulated user accounts, group assignments, and permissions to determine whether access aligns with business responsibilities.
-  **Evidence Required:** User and group inventories, policy attachments, and access review results.
-  **Result:** Not yet assessed.
-  **Findings:** Pending evidence collection.
-  **Recommended Action:** Document account ownership, review permissions regularly, and remove unnecessary access.

# Control 3: Multi-Factor Authentication
- **Control Objective:** Reduce the risk of unauthorized access through stronger authentication.
- **Framework Reference:** NIST SP 800-53 IA-2 - Identification and Authentication (for Organizational User).
- **Assessment Procedure:** Review the configured MFA status for relevant accounts and evaluate authentication requirements for privileged access. 
-  **Evidence Required:** Available MFA configuration details and documented verification results. 
-  **Result:** Not yet assessed.
-  **Findings:** Pending evidence collection.
-  **Recommended Action:** Address missing MFA protections and verify that applicable authentication requirements are met.

# Control 4: Audit Logging
- **Control Objective:** Maintian records of relevant account activity and security related events. 
- **Framework Reference:** NIST SP 800-53 AU-2 - Event Logging.
- **Assessment Procedure:** Review the available audit logging configuration and determine whether relevant IAM and account activities are recorded.
-  **Evidence Required:** Logging configuration details and sample audit events where available. 
-  **Result:** Not yet assessed.
-  **Findings:** Pending evidence collection.
-  **Recommended Action:** Address gaps in audit logging and document an appropriate monitoring and review process.

# Assessment Notes
Control reference identify relevant areas of the NIST SP 800-53 framework. Their inclusion does not establish that a control has been implemented or that the environment is compliant. The Final conclusions will be dependent on the evidence collected and the assessment scope. 

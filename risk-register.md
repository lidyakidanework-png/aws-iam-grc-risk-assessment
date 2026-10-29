# AWS IAM Risk Register 
# Purpose 
This risk register documents potential identity and access management risks identified for assessment in the simulated AWS environment. Each risk will be evaluated based on likelihood, business impact, existing controls and recommended remediation. 

# Risk Assessment Criteria 
**- Likelihood:** Low, Medium, or High 
**- Impact:** Low, Medium, or High 
**- Risk Rating:** To be determined after assessing likelihood and impact 
**- Status:** Open until the risk has been evaluated and appropriate actions documented 

#Initial Risk for Assessment 
# Risk-001: Excessive IAM Permissions
- **Risk Description:** Users may have permissions beyond those required for their job responsibilities, potentially allowing unauthorized access to AWS resources
**- Affected Asset:** AWS IAM users, groups, and policies.
**- Likelihood:** To be assessed.
**- Impact:** To be assessed. 
**- Risk Rating:** Pending assessment.
**- Existing Controls:** To be verified.
**- Recommended Mitigation:** Apply least privilege access, review attached policies, and remove unnecessary permissions. 
**- Status:** Open - assessment pending. 

# Risk-002: Inadequate Multi-Factor Authentication
**- Risk Description:** Accounts without appropriate MFA protection may be more vulnerable to unauthorized access if credentials are compromised. 
**- Affected Asset:** AWS IAM user accounts 
**- Likelihood:** To be assessed. 
**- Impact:** To be assessed. 
**- Risk Rating:** To be assessed. 
**- Existing Controls:** To be verified. 
**- Recommended Mitigations:** Review MFA enrollment and enforce appropriate authentication requirements, especially for privileged access. 
**- Status:** Open - assessment pending 

# Risk-003: Insufficient Access Monitoring
**- Risk Description:** Insufficient logging or review of account activity may delay detection of unauthorized access or inappropriate permission changes. 
**- Affected Asset:** AWS account activity, IAM changes, and access related events. 
**- Likelihood:** To be assessed. 
**- Impact:** To be assessed. 
**- Risk Rating:** To be assessed. 
**- Existing Controls:** To be verified. 
**- Recommended Mitigations:** Review available AWS audit logging, validate monitoring coverage, and establish a process for reviewing relevant  events. 
**- Status:** Open - assessment pending. 

The Next Steps: 
- Inspect the existing AWS IAM configurations.
- Gather evidence for each risk.
- Determine likelihood, impact, and risk ratings.
- Document verified existing controls.
- Record remediation actions and track unresolved risks. 

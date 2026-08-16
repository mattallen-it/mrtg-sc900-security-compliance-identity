# Lab 04 - RBAC and Conditional Access

> **Status:** Complete

## AI Use Disclosure

AI tools may be used to support learning, troubleshooting, documentation organization, technical review, and GitHub formatting during this lab.

All hands-on configuration, validation, screenshots, administrative decisions, and final documentation review must be completed by the project author. AI-generated guidance must be reviewed against Microsoft documentation and the observed behavior of the lab environment before being accepted.

---

## Lab Metadata

| Item | Value |
|---|---|
| Difficulty | Beginner |
| Estimated Time | 2-3 hours |
| Lab Type | Microsoft Learn + read-only discovery |
| SC-900 Domain | Describe the capabilities of Microsoft Entra |
| Primary Objective | Describe access management capabilities of Microsoft Entra |
| Previous Lab Dependency | Lab 03 - Authentication and Multifactor Authentication |
| Next Lab Dependency | Lab 05 - Identity Governance |

---

## Objective

Build a practical understanding of Microsoft Entra access-management capabilities and explain how authorization, least privilege, Conditional Access, role-based access control, and Global Secure Access support Zero Trust.

This lab focused on the Microsoft Learn module **Describe access management capabilities of Microsoft Entra** and covered:

- Authorization and least privilege
- Microsoft Entra administrative roles
- Role-based access control concepts
- Microsoft Entra roles vs. Azure RBAC
- Conditional Access signals and decisions
- Conditional Access assignments and access controls
- Authentication strength concepts
- Global Secure Access
- Microsoft Entra Internet Access and Microsoft Entra Private Access concepts
- Zero Trust access decision making

Identity governance, Privileged Identity Management, access reviews, entitlement management, and identity-risk capabilities are intentionally deferred to Lab 05.

---

## Business Problem Solved

Monroe Redstone Technology Group (MRTG) needs to ensure that authenticated identities receive only the access required for their responsibilities and that access is allowed only under appropriate conditions.

Without a strong access-management strategy, MRTG could experience:

- Excessive administrative permissions
- Standing privilege that is broader than required
- Confusion between authentication and authorization
- Misuse of Microsoft Entra roles or Azure RBAC
- Access from risky locations, devices, or sessions
- Inconsistent enforcement of MFA and device requirements
- Weak separation between identity administration and Azure resource administration
- Poor alignment with least privilege and Zero Trust

---

## Scenario

MRTG has already established identity and authentication fundamentals. The organization must now understand how Microsoft Entra controls what authenticated identities are allowed to do and under what conditions access should be granted.

The security team reviewed Microsoft Entra administrative roles, Azure RBAC concepts, Conditional Access, and Global Secure Access. The lab combined Microsoft Learn with sanitized read-only discovery in the Microsoft Entra admin center.

This was a discovery-focused lab. No production roles, Conditional Access policies, or Global Secure Access configurations were created or modified solely for portfolio evidence.

---

## Success Criteria

The lab was successful because:

- The Microsoft Learn module **Describe access management capabilities of Microsoft Entra** was completed
- The module assessment was passed
- Authentication and authorization were distinguished correctly
- Least privilege was applied to access-management scenarios
- Microsoft Entra roles were distinguished from Azure RBAC
- Conditional Access signals and access decisions were explained
- Conditional Access was distinguished from RBAC
- Global Secure Access was recognized as an access-security capability
- Microsoft Entra administrative areas were explored without unnecessary configuration changes
- Scenario-based knowledge checks were completed successfully
- The screenshot set was reviewed and uploaded to GitHub

---

## Prerequisites

- Completed Lab 03
- Access to Microsoft Learn
- General Microsoft Entra ID fundamentals
- General authentication and MFA fundamentals
- Access to the Microsoft Entra admin center for read-only discovery
- Access to the project GitHub repository

---

## Expected Starting State

- Lab 03 complete
- No Lab 04 role assignments or Conditional Access changes performed
- Microsoft Learn **Introduction to Microsoft Entra** learning path available
- Microsoft Entra admin center available for discovery
- No requirement to create privileged assignments for evidence

---

## Required Permissions

| Permission or Role | Purpose | Required |
|---|---|---|
| Microsoft Learn account | Complete module and assessment | Yes |
| Microsoft Entra tenant access | Read-only access-management discovery | Recommended |
| Privileged Microsoft Entra role | Not required for core lab | No |
| Azure subscription role assignment | Not required for core lab | No |

Least privilege was maintained. No privilege elevation was required solely for screenshot capture or administrative discovery.

---

## Microsoft Services and Resources Used

| Service or Resource | Purpose |
|---|---|
| Microsoft Learn | SC-900 access-management training and assessment |
| Microsoft Entra admin center | Read-only review of roles, Conditional Access, and Global Secure Access |
| GitHub | Documentation and sanitized evidence storage |

---

## Why These Services Were Used

Microsoft Learn provided certification-aligned instruction for Microsoft Entra access-management capabilities. The Microsoft Entra admin center connected the concepts to the administrative interface used by identity and security teams. GitHub provided a version-controlled portfolio record of the lab.

---

## Environment

```text
Organization: Monroe Redstone Technology Group (MRTG)
Lab mode: Microsoft Learn + read-only discovery
Microsoft Entra role assignments created: None
Azure RBAC assignments created: None
Conditional Access policies created or modified: None
Global Secure Access configuration changes: None
Azure consumption resources deployed: None
Estimated Azure consumption cost: $0.00
```

---

## Architecture / Concept Diagram

```text
Authenticated identity
        |
        v
Access request
        |
        +------------------------------+
        |                              |
        v                              v
Authorization                     Conditional Access
What can identity do?             Under what conditions?
        |                              |
        v                              +--> Identity / workload
Entra roles / Azure RBAC               +--> Device
        |                              +--> Location / network
        v                              +--> Risk
Least-privilege permissions             +--> Application / resource
        |                              |
        +---------------+--------------+
                        |
                        v
                 Access decision
                        |
          +-------------+-------------+
          |             |             |
        Allow        Require        Block
                    controls
```

This model separates **permission** from **access conditions**. RBAC defines what an identity is authorized to do, while Conditional Access evaluates contextual signals before access is allowed.

---

## Lab Safety and Change Control

- Confirmed the correct Microsoft Entra tenant before portal activity.
- Used read-only discovery for the administrative portion of the lab.
- Did not assign privileged roles solely for portfolio evidence.
- Did not create or enable Conditional Access policies solely for evidence.
- Did not modify Global Secure Access configuration.
- Avoided changing access controls that could create an administrative lockout.
- Did not publish user-specific role assignments or sensitive policy targeting information.
- Avoided exposing tenant IDs, object IDs, UPNs, administrative identities, secrets, tokens, or unnecessary security-posture details.
- Reviewed screenshots before publication.

---

## Steps Performed

1. Opened the Microsoft Learn module **Describe access management capabilities of Microsoft Entra**.
2. Reviewed Microsoft Entra administrative role concepts and role categories.
3. Reviewed least privilege and the relationship between roles, permissions, and scope.
4. Compared Microsoft Entra roles with Azure RBAC.
5. Reviewed Conditional Access as a policy engine that evaluates signals and applies access controls.
6. Reviewed Conditional Access signals such as identity, device, risk, application/resource, location, and network context.
7. Reviewed Conditional Access policy structure, including assignments, grant controls, and session controls.
8. Reviewed authentication-strength concepts within access decisions.
9. Reviewed Global Secure Access and its relationship to Microsoft Entra Internet Access and Microsoft Entra Private Access.
10. Passed the Microsoft Learn module assessment.
11. Completed scenario-based knowledge checks covering authorization, least privilege, roles, RBAC, Conditional Access, and Global Secure Access.
12. Performed read-only discovery in the Microsoft Entra admin center, including:
    - Entra ID > Roles & admins
    - Entra ID > Conditional Access
    - Global Secure Access
13. Uploaded and verified the final sanitized screenshot set in GitHub.

---

## Supporting Concept Summary

### Authentication vs. Authorization

| Concept | Purpose |
|---|---|
| Authentication | Verifies who or what an identity is |
| Authorization | Determines what the authenticated identity is permitted to access or do |

A user can authenticate successfully and still be denied access because authentication does not grant permission by itself.

### Least Privilege

Least privilege means assigning only the permissions necessary to perform a required task and limiting scope whenever practical.

A help desk technician who only needs password-reset capabilities should not receive a broad administrative role such as Global Administrator simply because it would technically allow the task.

### Microsoft Entra Roles vs. Azure RBAC

| Capability | Primary Purpose |
|---|---|
| Microsoft Entra roles | Administrative permissions for Microsoft Entra and related directory capabilities |
| Azure RBAC | Authorization for Azure resources and resource scopes |

The two systems both use role-based concepts, but they control different administrative planes.

### Conditional Access

Conditional Access evaluates access requests using signals and policy conditions. Depending on policy design, the result can be to allow access, require additional controls, restrict the session, or block access.

Common signals can include:

- User or workload identity
- Target application or resource
- Device state or compliance
- Location and network context
- Risk signals
- Authentication strength

### Conditional Access vs. RBAC

A useful mental model is:

```text
RBAC: What is this identity allowed to do?
Conditional Access: Under what conditions should this identity be allowed to access the resource?
```

These capabilities complement each other rather than replace one another.

### Global Secure Access

Global Secure Access brings together Microsoft Entra Internet Access and Microsoft Entra Private Access concepts to apply identity-aware access controls to public and private resources.

At an SC-900 level, the key point is that access security can extend beyond the traditional perimeter by combining identity, network, and policy context within a Zero Trust approach.

---

## Evidence Collected

| Screenshot | Evidence |
|---|---|
| `00-entra-access-management-module-starting-state.png` | Microsoft Learn access-management module starting state and objectives |
| `01-entra-roles-or-rbac.png` | Microsoft Entra role categories and role-based administrative concepts |
| `02-conditional-access-concept.png` | Conditional Access signals, continuous evaluation, and access decisions |
| `03-conditional-access-policy.png` | Conditional Access policy structure including assignments and access controls |
| `04-entra-access-management-module-complete.png` | Module assessment passed and module completion |

---

## Validation

| Validation Activity | Result |
|---|---|
| Microsoft Learn module completed | Passed |
| Microsoft Learn module assessment | Passed |
| Authentication vs. authorization knowledge check | Passed |
| Least-privilege scenario | Passed |
| Entra roles vs. Azure RBAC knowledge check | Passed |
| Conditional Access scenario | Passed |
| Conditional Access vs. RBAC knowledge check | Passed |
| Combined Conditional Access + least-privilege scenario | Passed |
| Global Secure Access knowledge check | Passed |
| Microsoft Entra read-only discovery | Completed |
| Repository screenshot verification | Completed |

Knowledge-check scenarios validated that:

- Authentication verifies identity, while authorization determines permitted access.
- Least privilege favors the narrowest role that satisfies the required task.
- Microsoft Entra roles manage directory and identity administration, while Azure RBAC manages access to Azure resources.
- Conditional Access evaluates signals and applies access decisions or controls.
- RBAC determines permissions, while Conditional Access governs conditions for access.
- Strong authentication and trusted-device requirements can be combined with least-privilege role assignments.
- Global Secure Access supports identity-aware access to public and private resources.

---

## Completion Checklist

- [x] Capture starting-state screenshot
- [x] Complete Microsoft Entra roles section
- [x] Review RBAC concepts
- [x] Review least-privilege concepts
- [x] Complete Conditional Access section
- [x] Review Conditional Access signals and policy controls
- [x] Review authentication-strength concepts
- [x] Review Global Secure Access
- [x] Pass module assessment
- [x] Perform sanitized Entra roles discovery
- [x] Perform sanitized Conditional Access discovery
- [x] Perform sanitized Global Secure Access discovery
- [x] Complete authentication vs. authorization knowledge check
- [x] Complete least-privilege knowledge check
- [x] Complete Entra roles vs. Azure RBAC knowledge check
- [x] Complete Conditional Access knowledge checks
- [x] Complete Global Secure Access knowledge check
- [x] Upload sanitized screenshots
- [x] Perform final repository evidence review
- [x] Mark Lab 04 complete

---

## SC-900 Exam Objective Coverage

### Primary Exam Domain

```text
Describe the capabilities of Microsoft Entra
```

### Primary Skill Area

```text
Describe access management capabilities of Microsoft Entra
```

This lab covered access-management concepts including:

- Conditional Access
- Microsoft Entra roles
- Role-based access control concepts
- Global Secure Access
- Least privilege and Zero Trust access decisions

---

## Mini Objective Coverage

| Objective | Coverage |
|---|---|
| Authorization | Distinguished authorization from authentication |
| Least privilege | Applied narrow-role reasoning to administrative scenarios |
| Microsoft Entra roles | Reviewed role categories and administrative purpose |
| Azure RBAC | Distinguished Azure resource authorization from Entra directory roles |
| Conditional Access | Reviewed signals, assignments, grant/session controls, and access outcomes |
| Authentication strength | Connected stronger authentication requirements to Conditional Access decisions |
| Global Secure Access | Reviewed the identity-aware access-security concept for public and private resources |
| Administrative discovery | Reviewed roles, Conditional Access, and Global Secure Access without changing configuration |

---

## Exam Traps and Key Distinctions

- Authentication and authorization are not the same thing.
- Successful authentication does not automatically grant permission to a resource.
- Microsoft Entra roles and Azure RBAC are separate authorization systems with different primary scopes.
- Global Administrator is not the correct default role simply because it can perform a task.
- Least privilege means selecting the narrowest practical permission and scope.
- Conditional Access does not assign Azure RBAC roles.
- RBAC does not replace MFA or Conditional Access.
- Conditional Access evaluates conditions for access; RBAC defines authorized actions.
- A Conditional Access policy can require additional controls or block access based on evaluated conditions.
- Global Secure Access is not another name for Azure RBAC or Conditional Access.
- Strong authentication is only one part of access security; permissions and context still matter.

---

## IAM / Security Relevance

This lab represents a core IAM transition from **proving identity** to **controlling access**.

A practical access-management model asks:

```text
Who is requesting access?
What is the identity allowed to do?
What scope does that permission apply to?
Under what conditions should access be allowed?
```

Microsoft Entra roles, Azure RBAC, Conditional Access, and Global Secure Access address different parts of those questions.

---

## On-Premises Connection

Traditional Active Directory environments commonly use security groups, delegated permissions, Group Policy, and network controls to manage authorization and access conditions.

Microsoft Entra extends access management into cloud identities, SaaS applications, Azure resources, device and risk signals, and identity-aware network access. Hybrid environments therefore require administrators to understand both on-premises authorization models and cloud access controls.

---

## Security Analysis

Broad permissions and weak access conditions can turn a single compromised identity into a larger security incident.

MRTG should reduce this risk by:

- Assigning only necessary administrative permissions
- Limiting assignment scope where possible
- Separating identity administration from Azure resource administration when duties differ
- Using Conditional Access to evaluate contextual access signals
- Requiring stronger authentication for higher-risk scenarios
- Using device, location, network, and risk context where appropriate
- Monitoring privileged access and policy changes
- Avoiding permanent broad privilege when narrower approaches are available

---

## Zero Trust Analysis

Lab 04 maps directly to all three Zero Trust principles:

- **Verify explicitly:** evaluate identity, authentication strength, device, risk, location, network, and resource context.
- **Use least-privilege access:** grant only required roles and permissions at the narrowest practical scope.
- **Assume breach:** design access so that one compromised credential, device, or session does not automatically provide unrestricted access.

Conditional Access and role-based authorization solve different parts of the Zero Trust access problem and are strongest when used together.

---

## Governance and Compliance Notes

Access management should be governed through documented role definitions, approval processes, appropriate scopes, policy ownership, change control, and periodic review.

Regulated environments also benefit from auditable records showing who had administrative access, which policies controlled access, and how changes were approved and monitored.

Lab 05 will expand this foundation into lifecycle-oriented governance capabilities such as privileged access and access reviews.

---

## Cost and Licensing Considerations

```text
Estimated Azure consumption cost: $0.00
```

The core lab used Microsoft Learn and read-only Microsoft Entra discovery. No Azure consumption resources were deployed.

Conditional Access, Global Secure Access, and other advanced access-management capabilities can have licensing and tenant dependencies. The lab documented these capabilities conceptually and did not bypass licensing requirements solely to create portfolio evidence.

---

## Troubleshooting

No material technical issues were encountered during the core lab.

The primary safety consideration was avoiding unnecessary changes to privileged roles or access policies. Read-only discovery allowed the administrative interfaces to be reviewed without creating lockout risk or altering the tenant security posture.

---

## What I Would Do Differently in Production

A production access-management rollout should use staged design, testing, and change control rather than enabling broad policies immediately.

MRTG should:

- Inventory existing privileged role assignments
- Define administrative job functions and minimum required permissions
- Separate Microsoft Entra role requirements from Azure resource role requirements
- Maintain documented emergency-access procedures
- Pilot Conditional Access policies with controlled populations
- Use report-only or other safe validation approaches where available before enforcement
- Exclude emergency-access identities appropriately from policies when required by the organization's design
- Validate device, location, application, and authentication requirements before broad rollout
- Monitor sign-in and audit data after policy changes
- Document rollback procedures
- Review role assignments and access policies periodically

---

## Lessons Learned

- Authentication proves identity; authorization controls permitted actions.
- Least privilege depends on both permission level and scope.
- Microsoft Entra roles and Azure RBAC are related concepts but govern different administrative planes.
- Conditional Access is a contextual access-policy engine, not a role-assignment system.
- RBAC and Conditional Access work together: one defines permissions, while the other controls access conditions.
- Strong authentication does not replace least-privilege authorization.
- Global Secure Access extends identity-aware access concepts to public and private network resources.
- Read-only portal discovery can connect exam concepts to real administrative workflows without changing the security posture.

---

## Skills Demonstrated

- Microsoft Entra access-management fundamentals
- Authentication vs. authorization analysis
- Least-privilege reasoning
- Microsoft Entra role concepts
- Azure RBAC concepts
- Microsoft Entra roles vs. Azure RBAC comparison
- Conditional Access concepts
- Conditional Access signal analysis
- Conditional Access policy-structure analysis
- Authentication-strength concepts
- Global Secure Access concepts
- Zero Trust access reasoning
- Read-only Entra administrative discovery
- Security-conscious evidence collection
- Scenario-based SC-900 knowledge validation

---

## Cleanup

No role assignments, Conditional Access policies, Global Secure Access configurations, or Azure consumption resources were created during the core lab, so no technical cleanup was required.

Temporary evidence files outside the repository should be removed after sanitized versions are committed.

---

## Documentation Security Review

Final review confirmed that the published screenshot set does not intentionally expose:

- Personal email addresses or UPNs
- Tenant IDs or object IDs
- User-specific role assignments
- Privileged administrator identities
- Sensitive Conditional Access targeting details
- Secrets, tokens, or authentication credentials
- Unnecessary tenant security-posture information

The final evidence set was intentionally kept small and concept-focused.

---

## Screenshot Inventory

| Screenshot | Status | Purpose |
|---|---|---|
| `00-entra-access-management-module-starting-state.png` | Included | Starting state and module objectives |
| `01-entra-roles-or-rbac.png` | Included | Microsoft Entra role categories and administrative roles |
| `02-conditional-access-concept.png` | Included | Conditional Access signals and decision flow |
| `03-conditional-access-policy.png` | Included | Conditional Access policy structure |
| `04-entra-access-management-module-complete.png` | Included | Passed assessment and module completion |

---

## Outcome

Lab 04 successfully established the access-management foundation needed for deeper Microsoft Entra identity governance work.

MRTG can now distinguish authentication from authorization, apply least-privilege reasoning, differentiate Microsoft Entra roles from Azure RBAC, explain how Conditional Access evaluates contextual signals, and describe how Global Secure Access fits into a Zero Trust access strategy.

**Lab 04 status: Complete.**

---

## Next Lab

```text
Lab 05 - Identity Governance
```

Lab 05 will extend the access-management foundation into identity governance, privileged access, access reviews, entitlement concepts, identity lifecycle, and related Microsoft Entra governance capabilities.

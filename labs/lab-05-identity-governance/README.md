# Lab 05 - Identity Governance

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
| Primary Objective | Describe identity protection and governance capabilities of Microsoft Entra |
| Previous Lab Dependency | Lab 04 - RBAC and Conditional Access |
| Next Lab Dependency | Lab 06 - Azure Infrastructure Security |

---

## Objective

Build a practical understanding of Microsoft Entra identity governance and protection capabilities and explain how organizations can govern access over time, reduce standing privilege, review access, manage entitlement, detect risky identity activity, and support verifiable identity scenarios.

This lab focused on the Microsoft Learn module **Describe the identity protection and governance capabilities of Microsoft Entra** and covered:

- Microsoft Entra ID Governance
- Privileged Identity Management (PIM)
- Access reviews
- Entitlement management concepts
- Identity lifecycle concepts
- Microsoft Entra ID Protection
- User risk and sign-in risk
- Least privilege and just-in-time privilege
- Microsoft Entra Verified ID
- Microsoft Security Copilot integration with Microsoft Entra
- Governance of access over time

---

## Business Problem Solved

Monroe Redstone Technology Group (MRTG) needs to ensure that access is not only granted securely, but also reviewed, governed, risk-aware, and removed when it is no longer required.

Without identity governance and protection, MRTG could experience:

- Excessive standing privilege
- Stale user, guest, or privileged access
- Access that remains after job changes or departures
- Weak oversight of privileged roles
- Inconsistent access approvals
- Access creep over time
- Limited visibility into risky identities and sign-ins
- Poor evidence of access review and governance
- Weak controls around external access

---

## Scenario

MRTG has already established identity, authentication, role-based authorization, and Conditional Access fundamentals.

The organization must now understand how Microsoft Entra helps govern access throughout its lifecycle, reduce standing privilege, review access regularly, manage access packages, identify risky identity activity, and support verifiable digital identity scenarios.

This was a discovery-focused lab using Microsoft Learn and sanitized read-only exploration. No production privileged-role assignments, access-review campaigns, entitlement packages, risk policies, or Verified ID configurations were created solely for portfolio evidence.

---

## Success Criteria

The lab was successful because:

- The Microsoft Learn module **Describe the identity protection and governance capabilities of Microsoft Entra** was completed
- The module assessment was passed
- PIM was distinguished from permanent standing privilege
- Access reviews were explained as a recurring governance control
- Entitlement management was explained at an SC-900 level
- Identity lifecycle concepts were reviewed
- User risk and sign-in risk were distinguished
- Microsoft Entra Verified ID was reviewed conceptually
- Microsoft Security Copilot integration with Microsoft Entra was reviewed conceptually
- Read-only Entra governance discovery was completed
- Scenario-based knowledge checks were passed
- Evidence was sanitized, uploaded, and verified

---

## Prerequisites

- Completed Lab 04
- Access to Microsoft Learn
- General Microsoft Entra ID fundamentals
- Understanding of authentication, authorization, RBAC, and Conditional Access
- Access to the Microsoft Entra admin center for read-only discovery
- Access to the project GitHub repository

---

## Expected Starting State

- Lab 04 complete
- No Lab 05 privileged-role activations or governance changes performed
- Microsoft Learn identity protection and governance module available
- Microsoft Entra admin center available for discovery
- No requirement to create privileged assignments, access packages, or risk policies for evidence

---

## Required Permissions

| Permission or Role | Purpose | Required |
|---|---|---|
| Microsoft Learn account | Complete module and assessment | Yes |
| Microsoft Entra tenant access | Read-only governance discovery | Recommended |
| Privileged Microsoft Entra role | Not required for core lab | No |
| Azure subscription role assignment | Not required for core lab | No |

Least privilege was maintained. No privilege elevation was performed solely to complete the lab or capture portfolio evidence.

---

## Microsoft Services and Resources Used

| Service or Resource | Purpose |
|---|---|
| Microsoft Learn | SC-900 identity protection and governance training and assessment |
| Microsoft Entra admin center | Read-only review of governance and identity-protection capabilities |
| GitHub | Documentation and sanitized evidence storage |

---

## Why These Services Were Used

Microsoft Learn provided certification-aligned instruction for Microsoft Entra governance and identity-protection capabilities. The Microsoft Entra admin center connected the concepts to the administrative interface used by identity and security teams. GitHub provided a version-controlled portfolio record of the lab.

---

## Environment

```text
Organization: Monroe Redstone Technology Group (MRTG)
Lab mode: Microsoft Learn + read-only discovery
Privileged role assignments created: None
PIM activations performed for evidence: None
Access reviews created: None
Entitlement packages created: None
Identity Protection policies changed: None
Verified ID configurations created: None
Azure consumption resources deployed: None
Estimated Azure consumption cost: $0.00
```

---

## Architecture / Concept Diagram

```text
Identity receives access
        |
        v
Identity Governance
        |
        +--> PIM
        |     Just-in-time / time-bound privilege
        |
        +--> Access Reviews
        |     Recertify and remove stale access
        |
        +--> Entitlement Management
        |     Request / approval / assignment / expiration
        |
        +--> Identity Lifecycle
        |     Joiner / mover / leaver governance
        |
        +--> Identity Protection
              User risk / sign-in risk
                      |
                      v
             Investigation / remediation
```

Verified ID supports verifiable digital credential scenarios, while Security Copilot can assist identity and security teams with AI-supported analysis and investigation.

---

## Lab Safety and Change Control

- Confirmed the correct Microsoft Entra tenant before portal activity.
- Used read-only discovery for the administrative portion of the lab.
- Did not activate privileged roles solely for evidence.
- Did not create access reviews or access packages solely for evidence.
- Did not change Identity Protection or risk policies.
- Did not configure Verified ID solely for portfolio evidence.
- Did not publish risky-user details, risky sign-in details, privileged assignments, or user-specific governance information.
- Avoided exposing tenant IDs, object IDs, UPNs, administrative identities, secrets, tokens, or unnecessary security-posture details.
- Reviewed screenshots before publication.

---

## Steps Performed

1. Opened the Microsoft Learn module **Describe the identity protection and governance capabilities of Microsoft Entra**.
2. Reviewed Microsoft Entra ID Governance and the purpose of governing access over time.
3. Reviewed Privileged Identity Management and its just-in-time, time-bound, approval-based, visible, and auditable access controls.
4. Reviewed access reviews and how recurring reviews help validate group membership, application access, guest access, and privileged-role assignments.
5. Reviewed entitlement management and access-package concepts, including request, approval, assignment, review, expiration, and external-user governance.
6. Reviewed identity lifecycle concepts and the need to adjust access as users join, move within, or leave an organization.
7. Reviewed Microsoft Entra ID Protection and the relationship between risk signals, risky users, risky sign-ins, policy, investigation, and remediation.
8. Distinguished user risk from sign-in risk.
9. Reviewed Microsoft Entra Verified ID and verifiable digital credential concepts.
10. Reviewed Microsoft Security Copilot integration with Microsoft Entra at a conceptual level.
11. Passed the Microsoft Learn module assessment.
12. Completed scenario-based knowledge checks covering PIM, access reviews, entitlement management, Identity Protection, user risk vs. sign-in risk, Verified ID, and Security Copilot integration.
13. Performed read-only discovery in the Microsoft Entra admin center, including governance, PIM, access reviews, entitlement management, Identity Protection, and Verified ID areas where available.
14. Uploaded and verified the final sanitized screenshot set in GitHub.

---

## Supporting Concept Summary

### Privileged Identity Management

PIM reduces standing privilege by allowing privileged access to be controlled through mechanisms such as:

- Just-in-time activation
- Time-bound assignments
- Approval requirements
- Visibility and alerts
- Audit history

The security goal is to avoid leaving highly privileged permissions active indefinitely when they are only needed occasionally.

### Access Reviews

Access reviews provide a recurring process for deciding whether users, guests, group members, application users, or role holders still require their current access.

This helps reduce access creep and supports least privilege, governance, and auditability.

### Entitlement Management

Entitlement management helps automate access lifecycle processes through access packages and related policies.

At an SC-900 level, the key idea is that access can be requested, approved, assigned, reviewed, expired, and removed through a governed workflow rather than handled as an indefinite manual assignment.

### Identity Lifecycle

Identity governance should account for access changes across the user lifecycle:

```text
Joiner -> Mover -> Leaver
```

New users need appropriate initial access, role changes can require both new permissions and removal of old permissions, and departing users should have access removed promptly.

### Identity Protection

Microsoft Entra ID Protection uses identity-related risk signals to help identify potentially compromised users and suspicious authentication activity.

| Risk Type | Meaning |
|---|---|
| User risk | Likelihood that the identity itself is compromised |
| Sign-in risk | Likelihood that a specific authentication attempt is suspicious or unauthorized |

Risk information can support investigation, policy decisions, and remediation.

### Microsoft Entra Verified ID

Verified ID supports verifiable digital identity credentials that can be issued and verified in supported identity scenarios.

The key SC-900 concept is that identity attributes can be represented through verifiable credentials rather than relying only on traditional usernames and passwords.

### Microsoft Security Copilot Integration

Security Copilot can support identity and security teams by helping analyze identity-related information and accelerate investigation with AI-assisted context.

It supports human analysts and administrators; it does not replace governance controls, access reviews, Identity Protection, or administrative decision-making.

---

## Evidence Collected

| Screenshot | Evidence |
|---|---|
| `00-entra-identity-governance-module-starting-state.png` | Microsoft Learn module starting state and current learning objectives |
| `01-entra-privileged-identity-management.png` | PIM concepts including just-in-time, time-bound, approval-based, visible, and auditable privileged access |
| `02-entra-access-reviews.png` | Access review concepts for groups, applications, privileged roles, guest access, and recurring review |
| `03-entra-identity-protection-risk.png` | Identity Protection risk signals, risky users, risky sign-ins, investigation, and remediation flow |
| `04-entra-identity-governance-module-complete.png` | Module assessment passed and module completion |

---

## Validation

| Validation Activity | Result |
|---|---|
| Microsoft Learn module completed | Passed |
| Microsoft Learn module assessment | Passed |
| PIM knowledge check | Passed |
| Access review knowledge check | Passed |
| Entitlement management knowledge check | Passed |
| Identity Protection knowledge check | Passed |
| User risk vs. sign-in risk knowledge check | Passed |
| Privileged-access scenario | Passed |
| Verified ID knowledge check | Passed |
| Security Copilot integration knowledge check | Passed |
| Microsoft Entra read-only discovery | Completed |
| Repository screenshot verification | Completed |

Knowledge-check scenarios validated that:

- PIM supports just-in-time, time-bound, controlled privileged access.
- Access reviews help identify access that should no longer remain assigned.
- Entitlement management governs access through request, approval, assignment, review, and expiration workflows.
- Identity Protection evaluates user risk and sign-in risk using detected signals.
- User risk concerns the likelihood that an identity is compromised, while sign-in risk concerns a specific authentication attempt.
- PIM is the appropriate capability when elevated permissions should exist only when needed and under controlled conditions.
- Verified ID supports verifiable digital credentials.
- Security Copilot can assist identity and security teams with AI-supported analysis and investigation.

---

## Completion Checklist

- [x] Capture starting-state screenshot
- [x] Review PIM
- [x] Review access reviews
- [x] Review entitlement management
- [x] Review identity lifecycle concepts
- [x] Review Identity Protection
- [x] Distinguish user risk from sign-in risk
- [x] Review Verified ID
- [x] Review Security Copilot integration concept
- [x] Pass module assessment
- [x] Perform sanitized Entra governance discovery
- [x] Complete knowledge checks
- [x] Upload sanitized screenshots
- [x] Perform final repository evidence review
- [x] Mark Lab 05 complete

---

## SC-900 Exam Objective Coverage

### Primary Exam Domain

```text
Describe the capabilities of Microsoft Entra
```

### Primary Skill Area

```text
Describe identity protection and governance capabilities of Microsoft Entra
```

This lab covered identity protection and governance concepts including:

- Microsoft Entra ID Governance
- Privileged Identity Management
- Access reviews
- Entitlement management
- Identity lifecycle
- Microsoft Entra ID Protection
- User risk and sign-in risk
- Microsoft Entra Verified ID
- Microsoft Security Copilot integration with Microsoft Entra

---

## Mini Objective Coverage

| Objective | Coverage |
|---|---|
| Privileged Identity Management | Explained just-in-time and time-bound privileged access and reduced standing privilege |
| Access reviews | Explained recurring access recertification and removal of unnecessary access |
| Entitlement management | Reviewed access packages and governed access lifecycle concepts |
| Identity lifecycle | Connected access governance to joiner, mover, and leaver scenarios |
| Identity Protection | Reviewed risk signals, risky users, risky sign-ins, investigation, and remediation |
| User risk vs. sign-in risk | Distinguished identity-compromise likelihood from suspicious authentication-attempt likelihood |
| Verified ID | Reviewed verifiable digital credential concepts |
| Security Copilot integration | Reviewed AI-assisted identity and security investigation concepts |
| Administrative discovery | Reviewed governance and protection areas without changing tenant configuration |

---

## Exam Traps and Key Distinctions

- PIM is not the same as assigning permanent privileged access.
- PIM reduces standing privilege; it does not eliminate the need for role design or least privilege.
- Access reviews validate whether existing access is still needed; they are not the same as access-request workflows.
- Entitlement management governs access packages and access lifecycle; it is broader than a one-time role assignment.
- User risk and sign-in risk are different concepts.
- Identity Protection detects and evaluates identity risk; it does not replace Conditional Access or PIM.
- Verified ID is about verifiable credentials, not RBAC or password synchronization.
- Security Copilot assists analysts and administrators; it does not replace human approval, governance, or policy controls.
- Governance is continuous. Access should not remain indefinitely simply because it was once approved.

---

## IAM / Security Relevance

Identity governance addresses a critical IAM question:

```text
Should this identity still have this access, and if so, under what governance controls?
```

Authentication and authorization establish identity and permission. Governance adds lifecycle, review, privilege control, risk awareness, and evidence that access remains justified over time.

This is especially important for privileged identities, guests, contractors, role changes, and regulated environments where organizations may need to demonstrate how access is approved and reviewed.

---

## On-Premises Connection

Traditional Active Directory environments often rely on security-group membership, delegated administration, manual recertification, and account disablement during offboarding.

Microsoft Entra governance extends these ideas with cloud-based capabilities such as PIM, access reviews, entitlement management, identity-risk detection, and automated access lifecycle controls.

Hybrid environments still require disciplined lifecycle management across both on-premises and cloud identity systems.

---

## Security Analysis

Persistent privilege and stale access increase the blast radius of account compromise.

MRTG should reduce this risk by:

- Replacing unnecessary standing privilege with time-bound or just-in-time access where practical
- Reviewing privileged and sensitive access regularly
- Removing stale access promptly
- Governing guest and external-user access
- Using access packages and expiration where appropriate
- Monitoring risky users and risky sign-ins
- Escalating or remediating identity risk based on documented policy
- Protecting approval and recovery processes from abuse

---

## Zero Trust Analysis

Lab 05 reinforces all three Zero Trust principles:

- **Verify explicitly:** evaluate current identity risk and access context rather than assuming an identity remains trustworthy indefinitely.
- **Use least-privilege access:** reduce standing privilege and require only the access needed for the required duration.
- **Assume breach:** continuously review access and monitor identity risk because users, guests, credentials, and sessions can become compromised over time.

Governance adds a temporal dimension to Zero Trust: access that was correct yesterday may no longer be appropriate today.

---

## Governance and Compliance Notes

Identity governance should define:

- Who can request access
- Who approves access
- How long access remains valid
- Which access requires recurring review
- How privileged access is activated and audited
- How joiners, movers, and leavers are handled
- How guest and external-user access is governed
- How risky identities are investigated and remediated
- What evidence is retained for audit and compliance purposes

These controls are particularly valuable in regulated environments where organizations must demonstrate that access is authorized, reviewed, and removed appropriately.

---

## Cost and Licensing Considerations

```text
Estimated Azure consumption cost: $0.00
```

The core lab used Microsoft Learn and read-only Microsoft Entra discovery. No Azure consumption resources were deployed.

PIM, access reviews, entitlement management, Identity Protection, Verified ID, and Security Copilot integration can have licensing, tenant, or service dependencies. The lab documented unavailable or premium capabilities conceptually rather than bypassing licensing requirements solely to create portfolio evidence.

---

## Troubleshooting

No material technical issues were encountered during the core lab.

The primary constraint was avoiding disclosure of privileged assignments, risky-user details, risky sign-in details, and tenant-specific governance posture. Read-only discovery and concept-focused Microsoft Learn screenshots provided sufficient evidence without publishing sensitive administrative information.

---

## What I Would Do Differently in Production

A production identity-governance rollout should be staged and policy-driven.

MRTG should:

- Inventory current privileged and sensitive access
- Identify standing privilege that can move to PIM
- Define role activation requirements, duration, approvals, and notifications
- Establish recurring access reviews for privileged roles, guests, groups, and applications
- Design entitlement packages around business functions rather than ad hoc permissions
- Integrate governance with joiner, mover, and leaver processes
- Define risk-response procedures for risky users and risky sign-ins
- Assign clear owners for access reviews and access packages
- Monitor audit and sign-in activity
- Document emergency-access procedures
- Review licensing requirements before deployment

---

## Lessons Learned

- Access governance continues after access is initially granted.
- PIM reduces standing privilege by making privileged access temporary and controlled.
- Access reviews help prevent access creep and stale permissions.
- Entitlement management provides a governed access lifecycle rather than indefinite manual assignment.
- User risk and sign-in risk answer different security questions.
- Identity Protection adds risk awareness to identity security and access decisions.
- Verified ID represents a different identity model based on verifiable digital credentials.
- Security Copilot can assist identity investigation, but governance and administrative decisions remain human-controlled.
- Read-only portal discovery can connect certification concepts to operational IAM workflows without altering tenant security posture.

---

## Skills Demonstrated

- Microsoft Entra identity governance fundamentals
- Privileged Identity Management concepts
- Just-in-time and time-bound privilege analysis
- Access review concepts
- Entitlement management concepts
- Identity lifecycle analysis
- Microsoft Entra ID Protection concepts
- User risk vs. sign-in risk analysis
- Microsoft Entra Verified ID concepts
- Microsoft Security Copilot integration concepts
- Least-privilege governance reasoning
- Zero Trust governance analysis
- Read-only Entra administrative discovery
- Security-conscious evidence collection
- Scenario-based SC-900 knowledge validation

---

## Cleanup

No privileged-role activations, access reviews, access packages, Identity Protection policy changes, Verified ID configurations, or Azure consumption resources were created during the core lab, so no technical cleanup was required.

Temporary evidence files outside the repository should be removed after sanitized versions are committed.

---

## Documentation Security Review

Final review confirmed that the published screenshot set does not intentionally expose:

- Personal email addresses or UPNs
- Tenant IDs or object IDs
- Privileged administrator identities
- User-specific role assignments
- Risky-user identities
- Risky sign-in details
- Secrets, tokens, or authentication credentials
- Unnecessary tenant security-posture information

The final evidence set was intentionally kept small and concept-focused.

---

## Screenshot Inventory

| Screenshot | Status | Purpose |
|---|---|---|
| `00-entra-identity-governance-module-starting-state.png` | Included | Starting state and current module objectives |
| `01-entra-privileged-identity-management.png` | Included | PIM and controlled privileged access concepts |
| `02-entra-access-reviews.png` | Included | Access review and recurring recertification concepts |
| `03-entra-identity-protection-risk.png` | Included | Identity Protection risk evaluation and remediation flow |
| `04-entra-identity-governance-module-complete.png` | Included | Passed assessment and module completion |

---

## Outcome

Lab 05 successfully established the identity-protection and governance foundation needed to manage access beyond initial authentication and authorization.

MRTG can now explain how PIM reduces standing privilege, how access reviews and entitlement management govern access over time, how Identity Protection distinguishes user risk from sign-in risk, and how Verified ID and Security Copilot extend the Microsoft Entra identity ecosystem.

**Lab 05 status: Complete.**

---

## Next Lab

```text
Lab 06 - Azure Infrastructure Security
```

Lab 06 will shift from Microsoft Entra identity capabilities into Azure infrastructure security concepts including defense in depth, network protection, Azure Firewall, Web Application Firewall, DDoS Protection, Azure Bastion, Key Vault, and network security groups.

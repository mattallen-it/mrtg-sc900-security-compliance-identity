# Lab 05 - Identity Governance

> **Status:** In Progress

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
| Primary Objective | Describe identity governance capabilities of Microsoft Entra |
| Previous Lab Dependency | Lab 04 - RBAC and Conditional Access |
| Next Lab Dependency | Lab 06 - Azure Infrastructure Security |

---

## Objective

Build a practical understanding of Microsoft Entra identity governance capabilities and explain how organizations can manage privileged access, access reviews, entitlement, identity lifecycle, and identity risk.

This lab is expected to cover:

- Privileged Identity Management (PIM)
- Access reviews
- Entitlement management concepts
- Identity lifecycle concepts
- Microsoft Entra ID Protection concepts
- Identity risk and sign-in risk
- Least privilege and just-in-time privilege
- Governance of access over time

---

## Business Problem Solved

Monroe Redstone Technology Group (MRTG) needs to ensure that access is not only granted securely, but also reviewed, governed, and removed when it is no longer required.

Without identity governance, MRTG could experience:

- Excessive standing privilege
- Stale user or guest access
- Access that remains after job changes or departures
- Weak oversight of privileged roles
- Inconsistent access approvals
- Limited visibility into risky identities and sign-ins
- Poor evidence of access review and governance

---

## Scenario

MRTG has already established identity, authentication, role-based authorization, and Conditional Access fundamentals.

The organization must now understand how Microsoft Entra helps govern access throughout its lifecycle, reduce standing privilege, review access regularly, and identify risky identity activity.

This lab will use Microsoft Learn and sanitized read-only discovery. No production privileged-role assignments, access-review campaigns, entitlement packages, or risk policies will be created solely for portfolio evidence.

---

## Success Criteria

The lab will be considered successful when:

- The Microsoft Learn identity governance module is completed
- The module assessment is passed
- PIM can be distinguished from permanent role assignment
- Access reviews can be explained
- Entitlement management can be explained at an SC-900 level
- Identity lifecycle concepts can be described
- Identity risk and sign-in risk can be distinguished
- Read-only Entra governance discovery is completed
- Knowledge checks are passed
- Evidence is sanitized and uploaded

---

## Environment

```text
Organization: Monroe Redstone Technology Group (MRTG)
Lab mode: Microsoft Learn + read-only discovery
Privileged role assignments created: None
Access reviews created: None
Entitlement packages created: None
Identity Protection policies changed: None
Azure consumption resources deployed: None
Estimated Azure consumption cost: $0.00
```

---

## Planned Discovery Activities

Where tenant access and licensing allow, review these areas without changing configuration:

1. Microsoft Entra ID > Identity governance
2. Privileged Identity Management
3. Access reviews
4. Entitlement management
5. Identity Protection / risk-related areas

Do not create assignments, activate privileged roles, launch access reviews, create access packages, or change risk policies solely for evidence.

---

## Planned Evidence

Keep the screenshot set small and useful:

| Screenshot | Evidence |
|---|---|
| `00-entra-identity-governance-module-starting-state.png` | Module starting state and objectives |
| `01-entra-privileged-identity-management.png` | PIM / just-in-time privileged access concept |
| `02-entra-access-reviews-or-entitlement.png` | Access reviews or entitlement management concept |
| `03-entra-identity-protection-risk.png` | Identity Protection / identity risk concept |
| `04-entra-identity-governance-module-complete.png` | Module assessment passed and completion |

Only screenshots actually captured and sanitized will remain in the final README.

---

## Completion Checklist

- [ ] Capture starting-state screenshot
- [ ] Review PIM
- [ ] Review access reviews
- [ ] Review entitlement management
- [ ] Review identity lifecycle concepts
- [ ] Review Identity Protection
- [ ] Distinguish identity risk from sign-in risk
- [ ] Pass module assessment
- [ ] Perform sanitized Entra governance discovery
- [ ] Complete knowledge checks
- [ ] Upload sanitized screenshots
- [ ] Perform final repository evidence review
- [ ] Mark Lab 05 complete

---

## IAM / Security Relevance

Identity governance addresses a critical IAM question:

```text
Should this identity still have this access, and if so, under what governance controls?
```

Authentication and authorization are only part of access management. Governance adds lifecycle, review, privilege control, and risk awareness so that access does not remain indefinitely without justification.

---

## Cost and Licensing Considerations

```text
Estimated Azure consumption cost: $0.00
```

No Azure consumption resources are required for the core lab.

PIM, access reviews, entitlement management, and Identity Protection can depend on Microsoft Entra licensing. Any unavailable premium capability will be documented rather than bypassed solely to complete the lab.

---

## Screenshot Inventory

To be completed after final evidence selection.

---

## Next Lab

```text
Lab 06 - Azure Infrastructure Security
```

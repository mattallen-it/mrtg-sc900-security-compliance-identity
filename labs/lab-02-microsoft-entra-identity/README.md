# Lab 02 - Microsoft Entra Identity

> **Status:** In Progress

## AI Use Disclosure

AI tools may be used to support learning, troubleshooting, documentation organization, and technical review during this lab. All hands-on work, validation, screenshots, administrative decisions, and final documentation review will be completed by the project author. AI-generated guidance will be reviewed against Microsoft documentation and observed lab results before being accepted.

---

## Lab Metadata

| Item | Value |
|---|---|
| Difficulty | Beginner |
| Estimated Time | 2-3 hours |
| Lab Type | Microsoft Learn + discovery |
| SC-900 Domain | Describe the capabilities of Microsoft Entra |
| Primary Objective | Describe function and identity types of Microsoft Entra ID |
| Previous Lab Dependency | Lab 01 - Security, Compliance, and Identity Foundations |
| Next Lab Dependency | Lab 03 - Authentication and Multifactor Authentication |

---

## Objective

Build a practical understanding of Microsoft Entra ID as Microsoft's cloud identity and access management platform and distinguish the major identity types it supports.

This lab focuses on the first module of the **Introduction to Microsoft Entra** learning path and covers:

- Microsoft Entra and the function of Microsoft Entra ID
- User identities
- Device identities
- Workload identities
- Applications and service principals
- Managed identities
- Microsoft Entra Agent ID and agent identities
- Groups
- Hybrid identity
- Microsoft Entra External ID and external identities

Authentication methods, MFA, Conditional Access, RBAC, identity protection, and identity governance are intentionally deferred to Labs 03-05 so each topic receives focused treatment.

---

## Business Problem Solved

Monroe Redstone Technology Group (MRTG) needs to understand the identity objects that exist in Microsoft Entra before it can safely design authentication, authorization, governance, or monitoring controls.

Without this foundation, MRTG could:

- Treat every identity as if it represents a human user
- Misunderstand how applications and services authenticate
- Confuse device identities with user identities
- Create unnecessary credentials instead of using managed identities
- Mismanage external collaboration
- Fail to account for hybrid identities spanning AD DS and Microsoft Entra ID
- Overlook emerging AI agent identities and their governance requirements

---

## Scenario

MRTG is reviewing its cloud identity architecture before implementing stronger authentication and access policies.

The organization must identify the different identity categories that may request access to resources and understand how Microsoft Entra ID represents people, devices, workloads, external users, hybrid users, and AI agents.

The lab combines Microsoft Learn with sanitized discovery in the Microsoft Entra admin center where useful. No production identities or access policies should be modified solely for evidence collection.

---

## Success Criteria

The lab is successful when:

- The Microsoft Learn module **Describe the function and identity types of Microsoft Entra ID** is completed
- Microsoft Entra ID can be described in practical IAM terms
- User, device, workload, external, hybrid, and agent identities can be distinguished
- Applications, service principals, and managed identities can be differentiated
- System-assigned and user-assigned managed identities can be explained
- Security groups and Microsoft 365 groups can be distinguished at a foundational level
- Hybrid identity can be explained as a common identity spanning on-premises and cloud environments
- External ID can be related to B2B collaboration and customer/external access scenarios
- Screenshots are sanitized before publication

---

## Prerequisites

- Completed Lab 01
- Access to Microsoft Learn
- General Azure and Microsoft 365 fundamentals
- Access to the Microsoft Entra admin center for optional discovery
- Access to the project GitHub repository

---

## Expected Starting State

- Lab 01 complete
- No Lab 02 configuration changes performed yet
- Microsoft Learn **Introduction to Microsoft Entra** learning path available
- No requirement to create real personal identities for evidence

---

## Required Permissions

| Permission or Role | Purpose | Required |
|---|---|---|
| Microsoft Learn account | Complete module and assessment | Yes |
| Microsoft Entra tenant access | Read-only/discovery activities | Recommended |
| Privileged Entra role | Not required for core lab | No |

Use the least privilege available. Do not elevate permissions simply to capture screenshots.

---

## Microsoft Learn Content

### Learning Path

**Introduction to Microsoft Entra**

This learning path currently contains four modules. The SC-900 lab series divides them across Labs 02-05:

1. **Lab 02** - Describe the function and identity types of Microsoft Entra ID
2. **Lab 03** - Describe the authentication capabilities of Microsoft Entra ID
3. **Lab 04** - Describe access management capabilities of Microsoft Entra
4. **Lab 05** - Describe the identity protection and governance capabilities of Microsoft Entra

### Lab 02 Module

Complete **Describe the function and identity types of Microsoft Entra ID**.

Review:

- Microsoft Entra
- Microsoft Entra ID
- Identity types
- Microsoft Entra Agent ID
- Hybrid identity
- External identities
- Module assessment

---

## Discovery Activities

Where tenant access is available, perform sanitized read-only exploration of:

1. Microsoft Entra admin center overview
2. **Identity > Users**
3. **Identity > Groups**
4. **Identity > Devices** where available
5. **Applications > Enterprise applications** to connect workload identity concepts to service principals
6. **External Identities** to identify the collaboration/external access area

Do not expose real names, personal email addresses, user principal names, tenant IDs, object IDs, or unrelated tenant information in published screenshots.

---

## Concept Work to Produce

The completed Lab 02 documentation will include:

1. **Identity Type Matrix** - user, device, workload, external, hybrid, and agent identity
2. **Application Identity Flow** - application registration -> service principal -> resource access
3. **Managed Identity Comparison** - system-assigned vs user-assigned
4. **Group Comparison** - security group vs Microsoft 365 group
5. **Hybrid Identity Summary** - AD DS to Microsoft Entra ID provisioning/synchronization concept
6. **External Identity Summary** - workforce B2B collaboration vs external/customer identity scenarios
7. **Agent Identity Security Note** - why AI agents need governed identities and least privilege

---

## Planned Evidence

Keep the screenshot set small and useful:

| Screenshot | Evidence |
|---|---|
| `00-entra-learning-path-starting-state.png` | Introduction to Microsoft Entra learning-path starting state |
| `01-entra-admin-center-overview.png` | Sanitized Microsoft Entra admin center discovery |
| `02-entra-identity-types.png` | Microsoft Learn identity-types content or other strong identity-type evidence |
| `03-hybrid-or-external-identity.png` | Strong visual for hybrid identity or External ID; choose the better evidence rather than capturing both without need |
| `04-entra-function-identity-types-module-complete.png` | Passed module assessment and module completion |

Only screenshots actually captured and sanitized will remain in the final README.

---

## Lab Safety and Change Control

- Confirm the correct Microsoft Entra tenant before any portal activity.
- Prefer read-only discovery for this lab.
- Do not create real personal accounts solely for portfolio evidence.
- Do not assign privileged roles for screenshot purposes.
- Do not publish personal names, email addresses, UPNs, tenant IDs, object IDs, secrets, tokens, or authentication details.
- Use fictional MRTG identities where hands-on examples are needed.
- Sanitize all screenshots before committing them to GitHub.
- Treat AI-generated guidance as secondary to Microsoft documentation and observed results.

---

## Cost and Licensing Considerations

```text
Estimated Azure consumption cost: $0.00
```

The core lab uses Microsoft Learn and read-only Microsoft Entra discovery. No Azure consumption resources are required.

Some Microsoft Entra capabilities discussed later in the series may require premium licensing, but premium licensing is not required simply to understand the identity types covered in this lab.

---

## SC-900 Exam Objective Coverage

### Primary Exam Domain

```text
Describe the capabilities of Microsoft Entra
```

### Primary Skill Area

```text
Describe function and identity types of Microsoft Entra ID
```

This lab supports the ability to:

- Describe Microsoft Entra ID
- Describe types of identities, including agent ID
- Describe hybrid identity

The Microsoft Learn module also introduces external identities and Microsoft Entra External ID as supporting identity concepts.

---

## IAM / Security Relevance

A core IAM question is:

```text
Who or what is requesting access?
```

In Microsoft Entra, the answer may be a human user, device, application, managed identity, external identity, hybrid identity, or AI agent. Correctly identifying the identity type is necessary before selecting authentication, authorization, governance, and monitoring controls.

---

## Zero Trust Connection

Lab 02 applies Zero Trust by refusing to assume that all identities deserve the same level or type of access.

- **Verify explicitly:** understand what identity is authenticating and the signals available for that identity type.
- **Use least privilege:** assign only the permissions required by the user, workload, device, external user, or agent.
- **Assume breach:** design identity lifecycle and monitoring with the expectation that any identity type could be compromised or misused.

---

## Completion Checklist

- [ ] Capture starting-state screenshot
- [ ] Complete Microsoft Entra identity-types module
- [ ] Pass module assessment
- [ ] Perform sanitized Entra admin center discovery
- [ ] Complete identity-type knowledge checks
- [ ] Complete application/service-principal knowledge check
- [ ] Complete managed-identity knowledge check
- [ ] Complete group knowledge check
- [ ] Complete hybrid-identity knowledge check
- [ ] Complete external-identity knowledge check
- [ ] Complete agent-identity knowledge check
- [ ] Upload sanitized screenshots
- [ ] Perform final repository evidence review
- [ ] Mark Lab 02 complete

---

## Next Lab

```text
Lab 03 - Authentication and Multifactor Authentication
```

Lab 03 will continue the Microsoft Entra learning path with authentication methods, MFA, password protection and management, and related authentication capabilities.

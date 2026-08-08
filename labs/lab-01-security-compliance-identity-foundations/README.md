# Lab 01 - Security, Compliance, and Identity Foundations

> **Status:** In Progress

## AI Use Disclosure

AI tools may be used to support learning, troubleshooting, documentation organization, and technical review during this lab. All hands-on work, validation, screenshots, administrative decisions, and final documentation review will be completed by the project author. AI-generated guidance will be reviewed against Microsoft documentation and observed lab results before being accepted.

---

## Lab Metadata

| Item | Value |
|---|---|
| Difficulty | Beginner |
| Estimated Time | 2-3 hours |
| Lab Type | Discovery-only |
| SC-900 Domain | Describe the concepts of security, compliance, and identity |
| Previous Lab Dependency | None |
| Next Lab Dependency | Lab 02 - Microsoft Entra Identity |

---

## Objective

Build a practical foundation in the security, compliance, and identity concepts that underpin the rest of the SC-900 series.

This lab is designed to cover the complete first SC-900 exam domain, including:

- Shared responsibility
- Defense in depth
- Confidentiality, integrity, and availability (CIA)
- Zero Trust
- Encryption and hashing
- Governance, Risk, and Compliance (GRC)
- Data residency, data sovereignty, and data privacy
- Identity as the primary security perimeter
- Authentication
- Authorization
- Identity providers
- Directory services and Active Directory
- Microsoft Entra ID as a cloud identity platform
- Federation

No Microsoft cloud resources, identities, roles, or policies will be created or modified during this lab.

---

## Business Problem Solved

Monroe Redstone Technology Group needs a common security and identity framework before implementing additional Microsoft cloud controls.

Without a shared foundation, MRTG could experience:

- Confusion over Microsoft versus customer security responsibilities
- Excessive trust in network location
- Weak identity-centered security decisions
- Inconsistent use of security terminology
- Poor understanding of data protection mechanisms
- Gaps between governance requirements and technical controls
- Incorrect assumptions about authentication and authorization
- Weak preparation for later Microsoft Entra, Defender, Sentinel, and Purview work

This lab establishes the concepts MRTG will use to make consistent identity, security, governance, and compliance decisions throughout the remaining series.

---

## Scenario

MRTG is preparing to expand its Microsoft cloud security program. Before configuring identity, access, threat protection, or compliance controls, the organization must define the security principles that will guide those decisions.

In this lab, MRTG must:

- Review the shared responsibility model across on-premises, IaaS, PaaS, SaaS, and AI-enabled services
- Map defense in depth and the CIA triad to the MRTG environment
- Apply the three Zero Trust principles and identify the seven technology pillars
- Distinguish encryption from hashing
- Review GRC, data residency, data sovereignty, and data privacy
- Distinguish identity, authentication, and authorization
- Review identity providers, directory services, Active Directory, Microsoft Entra ID, and federation
- Produce sanitized evidence demonstrating completion and understanding

```text
Discovery-only
```

> This is a discovery-only lab. No Microsoft cloud resources, identities, policies, roles, or security configurations are created or modified.

---

## Success Criteria

The lab is successful when:

- Both Microsoft Learn modules in the first SC-900 learning path are completed
- Shared responsibility can be explained across common service models
- The CIA triad and defense-in-depth concepts can be mapped to MRTG
- The three Zero Trust principles can be explained without relying on product names
- Encryption and hashing can be correctly distinguished
- GRC and data-location concepts can be explained in business terms
- Authentication and authorization can be correctly distinguished
- Identity provider, directory service, Active Directory, Microsoft Entra ID, and federation concepts can be explained
- Screenshots are captured and sanitized
- No tenant, subscription, user, billing, or authentication secrets are exposed

---

## Prerequisites

Before beginning this lab, confirm:

- Access to Microsoft Learn
- General Azure and cloud fundamentals knowledge
- Access to the MRTG Azure/Microsoft tenant for discovery where applicable
- Access to the project GitHub repository
- A local location for temporary screenshots before sanitization

No premium Microsoft license is required for the core learning activities in this lab.

---

## Required Permissions

| Permission or Role | Purpose | Required |
|---|---|---|
| Microsoft Learn account | Complete modules and assessments | Yes |
| Microsoft Entra tenant access | Optional discovery of the identity platform | Optional |
| Azure subscription access | Not required for configuration | No |

No privileged Microsoft Entra or Azure role is required for the core lab.

---

## Microsoft Learn Content

Complete the learning path **Introduction to security, compliance, and identity concepts**.

### Module 1 - Describe security and compliance concepts

Review:

- Shared responsibility
- Defense in depth
- Zero Trust
- Encryption and hashing
- Governance, Risk, and Compliance (GRC)
- Data residency, sovereignty, and privacy

### Module 2 - Describe identity concepts

Review:

- Authentication and authorization
- Identity as the primary security perimeter
- Identity providers
- Modern authentication and single sign-on concepts
- Directory services
- Active Directory Domain Services
- Microsoft Entra ID
- Federation

---

## Planned Evidence

| Screenshot | Evidence |
|---|---|
| `01-security-compliance-module-complete.png` | Completion of the security and compliance concepts module |
| `02-identity-concepts-module-complete.png` | Completion of the identity concepts module |
| `03-sc900-learning-path-progress.png` | Overall first learning-path completion/progress |
| `04-entra-platform-discovery.png` | Optional sanitized Microsoft Entra platform discovery |

Only screenshots that are actually captured will remain in the final README.

---

## Concept Work to Produce

The completed lab documentation will include:

1. **Shared Responsibility Matrix** - MRTG versus Microsoft responsibilities across service models.
2. **Defense-in-Depth / CIA Mapping** - How layered controls protect confidentiality, integrity, and availability.
3. **Zero Trust Mapping** - Verify explicitly, use least privilege, and assume breach across MRTG.
4. **Encryption vs Hashing Comparison** - Purpose, reversibility, and common security use.
5. **GRC Summary** - Governance, risk, compliance, data residency, sovereignty, and privacy.
6. **Identity Access Flow** - Identity -> Authentication -> Authorization -> Resource.
7. **Identity Platform Comparison** - Active Directory Domain Services versus Microsoft Entra ID.
8. **Federation Summary** - How trust between identity systems enables cross-boundary access.

---

## Lab Safety and Change Control

- Confirm the correct Microsoft Learn profile is being used.
- If opening a Microsoft tenant, confirm the correct tenant before capturing screenshots.
- Do not create or modify identities, roles, policies, or resources for this lab.
- Do not expose tenant IDs, subscription IDs, user principal names, personal email addresses, object IDs, authentication information, secrets, keys, or tokens.
- Sanitize every screenshot before publication.
- Treat AI-generated guidance as secondary to Microsoft documentation and observed results.

---

## Cost and Licensing Considerations

### Estimated Lab Cost

```text
Estimated cost: $0.00
```

This lab is intentionally discovery-only and does not require Azure consumption resources.

Azure Cost Management validation is not required because the lab does not deploy Azure resources.

---

## SC-900 Exam Objective Coverage

### Primary Exam Domain

```text
Describe the concepts of security, compliance, and identity
```

### Skills Measured

This lab supports the ability to:

- Describe the shared responsibility model
- Describe defense in depth
- Describe the Zero Trust model
- Describe encryption and hashing
- Describe Governance, Risk, and Compliance concepts
- Define identity as the primary security perimeter
- Define authentication
- Define authorization
- Describe identity providers
- Describe directory services and Active Directory
- Describe federation

---

## AI / Security Note

The current Microsoft Learn shared-responsibility material also applies the model to AI-enabled services. MRTG will treat AI use as governed organizational activity: Microsoft may secure the underlying service depending on the delivery model, while MRTG remains responsible for appropriate access, data handling, policy, user behavior, and validation of AI-generated output.

---

## Next Lab

The next lab is:

```text
Lab 02 - Microsoft Entra Identity
```

Lab 02 will move from foundational identity concepts into practical exploration of Microsoft Entra ID, identity types, users, groups, roles, and the MRTG cloud identity environment.

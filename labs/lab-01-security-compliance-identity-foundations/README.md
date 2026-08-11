# Lab 01 - Security, Compliance, and Identity Foundations

> **Status:** In Progress - concept work complete; screenshots pending repository upload

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

This lab covers:

- Shared responsibility
- Defense in depth
- Confidentiality, integrity, and availability (CIA)
- Zero Trust
- Encryption and hashing
- Governance, Risk, and Compliance (GRC)
- Data residency, data sovereignty, and data privacy
- Identity as a security perimeter
- Authentication
- Authorization
- Identity providers
- Directory services and Active Directory Domain Services (AD DS)
- Microsoft Entra ID as a cloud identity platform
- Federation

No Microsoft cloud resources, identities, roles, or policies were created or modified during this lab.

---

## Business Problem Solved

Monroe Redstone Technology Group (MRTG) needs a common security and identity framework before implementing additional Microsoft cloud controls.

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

The lab reviews shared responsibility across common service models, maps security concepts to practical MRTG scenarios, distinguishes identity and access concepts, and records sanitized evidence of Microsoft Learn completion.

```text
Discovery-only
```

> No Microsoft cloud resources, identities, policies, roles, or security configurations were created or modified.

---

## Success Criteria

The lab is successful when:

- Both Microsoft Learn modules in the first SC-900 learning path are completed
- Shared responsibility can be explained across on-premises, IaaS, PaaS, and SaaS
- The CIA triad can be mapped to practical business scenarios
- The three core Zero Trust principles can be explained
- Encryption and hashing can be correctly distinguished
- GRC and data-location concepts can be explained in business terms
- Authentication and authorization can be correctly distinguished
- AD DS and Microsoft Entra ID can be differentiated at a foundational level
- Federation can be explained as a trust relationship between identity systems
- Screenshots are captured and sanitized before publication

---

## Prerequisites

- Access to Microsoft Learn
- General Azure and cloud fundamentals knowledge
- Access to the project GitHub repository
- A local location for temporary screenshots before sanitization

No premium Microsoft license was required for the core activities in this lab.

---

## Expected Starting State

- SC-900 Microsoft Learn course available
- First learning path not yet completed
- No configuration changes planned
- Screenshot folder created in the repository

---

## Required Permissions

| Permission or Role | Purpose | Required |
|---|---|---|
| Microsoft Learn account | Complete modules and assessments | Yes |
| Microsoft Entra tenant access | Optional platform discovery | Optional |
| Azure subscription access | Not required for configuration | No |

No privileged Microsoft Entra or Azure role was required.

---

## Services and Resources Used

| Service or Resource | Purpose |
|---|---|
| Microsoft Learn | SC-900 learning content and module assessments |
| GitHub | Lab documentation and evidence organization |
| Microsoft Entra ID | Referenced as the Microsoft cloud identity platform; no changes performed |

---

## Why These Services Were Used

Microsoft Learn provided the official training material for the foundational SC-900 concepts. GitHub provides a version-controlled portfolio record of the work. Microsoft Entra ID is included conceptually because later labs build directly on the identity principles introduced here.

---

## Environment

```text
Organization: Monroe Redstone Technology Group (MRTG)
Lab mode: Discovery-only
Azure resources deployed: None
Identity changes performed: None
Estimated Azure consumption cost: $0.00
```

---

## Architecture / Concept Diagram

```text
Identity
   |
   v
Authentication
   |
   v
Authorization
   |
   v
Access to Resource

Security decisions surrounding the flow:
- Verify explicitly
- Use least privilege
- Assume breach
```

---

## Lab Safety and Change Control

- Confirm the correct Microsoft Learn profile is being used.
- Do not create or modify identities, roles, policies, or resources for this lab.
- Do not expose tenant IDs, subscription IDs, user principal names, personal email addresses, object IDs, authentication information, secrets, keys, or tokens.
- Sanitize every screenshot before publication.
- Treat AI-generated guidance as secondary to Microsoft documentation and observed results.

---

## Steps Performed

1. Opened the SC-900 course and recorded the starting state.
2. Completed **Describe security and compliance concepts**.
3. Reviewed the shared responsibility model across on-premises, IaaS, PaaS, and SaaS.
4. Reviewed defense in depth and the CIA triad.
5. Reviewed the Zero Trust principles: verify explicitly, use least privilege, and assume breach.
6. Distinguished encryption from hashing.
7. Reviewed governance, risk, compliance, data residency, data sovereignty, and data privacy.
8. Passed the security and compliance module assessment.
9. Completed **Describe identity concepts**.
10. Distinguished identity, authentication, authorization, and identity provider concepts.
11. Compared AD DS with Microsoft Entra ID at a foundational level.
12. Reviewed federation and trust relationships between identity systems.
13. Passed the identity concepts module assessment and completed the learning path.
14. Completed practical MRTG knowledge-check scenarios for each major concept area.

---

## Supporting Concept Summary

### Shared Responsibility

Cloud adoption changes which party manages portions of the technology stack, but it does not remove the customer's security responsibilities.

| Responsibility | On-Premises | IaaS | PaaS | SaaS |
|---|:---:|:---:|:---:|:---:|
| Information and data | MRTG | MRTG | MRTG | MRTG |
| Devices | MRTG | MRTG | MRTG | MRTG |
| Accounts and identities | MRTG | MRTG | MRTG | MRTG |
| Identity and directory infrastructure | MRTG | MRTG | Shared | Microsoft |
| Applications | MRTG | MRTG | Shared | Microsoft |
| Network controls | MRTG | MRTG | Shared | Microsoft |
| Operating system | MRTG | MRTG | Microsoft | Microsoft |
| Physical hosts | MRTG | Microsoft | Microsoft | Microsoft |
| Physical network | MRTG | Microsoft | Microsoft | Microsoft |
| Physical datacenter | MRTG | Microsoft | Microsoft | Microsoft |

Practical MRTG conclusions:

- If MRTG does not require appropriate authentication controls such as MFA and a user account is compromised, responsibility for protecting that identity remains with MRTG.
- Microsoft manages the underlying physical Azure infrastructure.
- For an Azure virtual machine, MRTG remains responsible for the guest operating system, including patching and configuration.
- Even in SaaS, MRTG controls its users, access decisions, and organizational data.

### Defense in Depth and the CIA Triad

Defense in depth uses multiple layers of controls so that the failure of one control does not result in complete compromise.

| CIA Principle | MRTG Example |
|---|---|
| Confidentiality | Only authorized HR personnel can view sensitive employee information |
| Integrity | Unauthorized modification of employee banking information must be prevented or detected |
| Availability | Authentication services must remain accessible so authorized employees can sign in |

### Zero Trust

| Principle | MRTG Application |
|---|---|
| Verify explicitly | Require appropriate authentication and evaluate available access signals before granting access |
| Use least privilege | Give a help desk technician only the permissions needed to perform the assigned task rather than broad administrator rights |
| Assume breach | Monitor sign-ins and design controls with the expectation that an account or device could become compromised |

### Encryption vs. Hashing

| Concept | Purpose | Reversible? | Example |
|---|---|:---:|---|
| Encryption | Protect information from unauthorized reading | Yes, with the proper key | Protecting a confidential file that an authorized user must later read |
| Hashing | Produce a one-way value for verification or secure representation | No | Verifying file integrity or storing password-derived values |

### Governance, Risk, Compliance, and Data Concepts

| Concept | MRTG Interpretation |
|---|---|
| Governance | Defines policies, responsibilities, direction, and required controls |
| Risk | Evaluates the likelihood and impact of potential harm |
| Compliance | Demonstrates that required laws, standards, or organizational requirements are being met |
| Data residency | Where data is physically stored |
| Data sovereignty | Which jurisdiction's laws apply to the data |
| Data privacy | How personal or sensitive information is collected, used, protected, and shared |

A useful distinction is:

```text
Residency   = Where is the data?
Sovereignty = Whose laws apply?
Privacy     = How is personal data handled?
```

### Identity, Authentication, and Authorization

```text
Identity       = Who the person, service, or object is
Authentication = Proving the claimed identity
Authorization  = Determining what the authenticated identity may do
```

An identity can authenticate successfully and still be denied access when it lacks the required authorization.

### Identity Provider

An identity provider authenticates an identity and provides trusted identity information that applications can use when making access decisions.

### AD DS vs. Microsoft Entra ID

| Active Directory Domain Services (AD DS) | Microsoft Entra ID |
|---|---|
| Traditional directory service commonly used for on-premises Windows domains | Cloud identity and access management service |
| Supports domain-joined environments and Group Policy | Supports cloud identities and access to Microsoft 365, Azure, and SaaS applications |
| Commonly uses Kerberos and NTLM in traditional domain scenarios | Supports modern authentication and cloud access scenarios |
| Designed around traditional domain resources | Designed for cloud identity and access management |

Microsoft Entra ID should not be treated as simply "Active Directory hosted in Azure." The technologies are related to identity management but have different architectures and use cases.

### Federation

Federation establishes a trust relationship between identity systems so that an organization can accept identities authenticated by another trusted organization or identity provider.

For MRTG, this can allow a partner user to access an approved MRTG application using the partner organization's existing identity instead of requiring MRTG to maintain a separate password for that user.

---

## Evidence Collected

The following evidence was captured during the lab and will be uploaded after final sanitization:

| Screenshot | Evidence |
|---|---|
| `00-sc900-course-starting-state.png` | SC-900 course and first learning-path starting state |
| `01-shared-responsibility-model.png` | Shared responsibility model across cloud service models |
| `02-security-compliance-module-complete.png` | Passed security and compliance concepts module assessment |
| `03-authentication-vs-authorization.png` | Microsoft Learn visual distinguishing authentication and authorization |
| `04-identity-concepts-and-learning-path-complete.png` | Passed identity concepts assessment and completed the learning path |

---

## Validation

Validation was performed through Microsoft Learn assessments and scenario-based knowledge checks.

| Validation Item | Result |
|---|---|
| Security and compliance concepts assessment | Passed |
| Identity concepts assessment | Passed |
| First SC-900 learning path | Completed |
| Shared responsibility scenarios | Correctly identified |
| CIA scenarios | Correctly identified |
| Zero Trust scenarios | Correctly identified |
| Encryption vs. hashing scenarios | Correctly identified |
| GRC/data concept scenarios | Correctly identified |
| Identity/authentication/authorization scenarios | Correctly identified |
| AD DS vs. Entra ID scenarios | Correctly identified |
| Federation scenario | Correctly identified |

---

## Completion Checklist

- [x] Completed security and compliance concepts module
- [x] Passed security and compliance module assessment
- [x] Completed identity concepts module
- [x] Passed identity concepts module assessment
- [x] Completed first SC-900 learning path
- [x] Completed shared responsibility knowledge check
- [x] Completed CIA knowledge check
- [x] Completed Zero Trust knowledge check
- [x] Completed encryption and hashing knowledge check
- [x] Completed GRC and data concepts knowledge check
- [x] Completed identity and access concepts knowledge check
- [x] Completed AD DS versus Entra ID knowledge check
- [x] Completed federation knowledge check
- [x] Captured required screenshots
- [ ] Upload sanitized screenshots to the repository
- [ ] Perform final repository evidence review

---

## SC-900 Exam Objective Coverage

### Primary Exam Domain

```text
Describe the concepts of security, compliance, and identity
```

This lab supports the ability to explain:

- Shared responsibility
- Defense in depth
- Confidentiality, integrity, and availability
- Zero Trust
- Encryption and hashing
- Governance, risk, and compliance
- Data residency, sovereignty, and privacy
- Identity as a security perimeter
- Authentication and authorization
- Identity providers
- Directory services and Active Directory
- Microsoft Entra ID at a foundational level
- Federation

---

## Mini Objective Coverage

| Objective | Demonstrated Through |
|---|---|
| Shared responsibility | Service-model matrix and MRTG scenarios |
| Defense in depth / CIA | Practical confidentiality, integrity, and availability scenarios |
| Zero Trust | Three-principle scenario mapping |
| Encryption / hashing | Security-use comparison |
| GRC and data concepts | Business scenario matching |
| Authentication / authorization | Identity access flow and practical scenario |
| Directory and identity platforms | AD DS versus Entra ID comparison |
| Federation | Cross-organization trust scenario |

---

## Exam Traps and Key Distinctions

- Cloud adoption does not transfer all security responsibility to Microsoft.
- Customer identities, accounts, devices, information, and data remain customer responsibilities across common cloud service models.
- Authentication answers **who are you?**; authorization answers **what are you allowed to do?**
- Encryption is designed to be reversible with the correct key; hashing is one-way.
- Data residency is about location; data sovereignty is about jurisdiction; data privacy is about handling personal information.
- Microsoft Entra ID is not simply AD DS running in Azure.
- Federation relies on trust between identity systems.

---

## IAM / Security Relevance

Identity is central to modern security because access decisions depend on knowing who or what is requesting access, validating that identity, and granting only the permissions required.

The concepts in this lab directly support later work with:

- Microsoft Entra authentication
- MFA
- Conditional Access
- Role-based access control
- Identity governance
- Security monitoring and investigation

---

## On-Premises Connection

Traditional AD DS environments commonly use Windows domains, domain joins, Group Policy, Kerberos, and NTLM. Microsoft Entra ID addresses cloud identity and access scenarios. Hybrid environments may use both, making the distinction important before designing or troubleshooting identity systems.

---

## Security Analysis

The largest foundational risks identified in this lab are not limited to technical vulnerabilities. They also include incorrect assumptions about responsibility and trust.

Examples include:

- Assuming Microsoft is responsible for all security after moving to SaaS
- Granting unnecessary administrative permissions
- Treating a successful password sign-in as sufficient proof for every access decision
- Failing to plan for compromise
- Confusing authentication with authorization
- Misunderstanding where organizational responsibility remains in cloud services

---

## Zero Trust Analysis

MRTG will carry the following model into later labs:

```text
Who or what is requesting access?
        |
        v
Verify explicitly
        |
        v
Grant only necessary access
        |
        v
Monitor with the assumption that compromise is possible
```

This provides a consistent security lens for future Microsoft Entra and security-control labs.

---

## Governance and Compliance Notes

Security controls should support business and regulatory requirements rather than exist in isolation. MRTG must understand what data it holds, where the data is stored, which legal or regulatory requirements apply, and how access and handling requirements are governed.

Later labs will connect these foundational concepts to Microsoft compliance capabilities.

---

## Cost and Licensing Considerations

```text
Estimated Azure consumption cost: $0.00
```

This lab was discovery-only and did not deploy Azure consumption resources. Azure Cost Management validation was therefore not required.

No premium Microsoft license was required for the core Microsoft Learn activities.

---

## Troubleshooting

No technical deployment issues occurred because this was a discovery-only lab.

The primary quality-control task was ensuring conceptual distinctions were understood correctly rather than merely completing Microsoft Learn pages.

---

## What I Would Do Differently in Production

In production, foundational concepts would be translated into documented organizational standards, including:

- Clearly assigned security responsibilities
- Formal access-control and least-privilege requirements
- Defined identity and authentication standards
- Risk-management processes
- Data-handling and privacy requirements
- Monitoring and incident-response expectations

The exact controls would depend on organizational risk, licensing, regulatory requirements, and technical architecture.

---

## Lessons Learned

- Moving to the cloud changes responsibility but does not eliminate customer responsibility.
- Identity remains a major customer security responsibility even in SaaS.
- Authentication and authorization solve different parts of the access-control process.
- Zero Trust is a security model rather than a single Microsoft product.
- Least privilege is directly applicable to administrative and help desk access.
- Encryption and hashing serve different purposes and should not be treated as interchangeable.
- Data location, legal jurisdiction, and privacy are related but distinct concepts.
- AD DS and Microsoft Entra ID are related identity technologies designed for different scenarios.
- Federation can reduce duplicate credential management by establishing trust between identity systems.

---

## Skills Demonstrated

- Security fundamentals analysis
- Shared responsibility analysis
- Zero Trust reasoning
- CIA triad application
- Identity and access management fundamentals
- Authentication versus authorization analysis
- Cloud versus traditional directory-service comparison
- Governance and compliance terminology
- Security documentation
- Evidence collection and sanitization planning

---

## Cleanup

No cloud resources or configurations were created, so no technical cleanup was required.

Temporary local screenshot copies should be removed after sanitized evidence has been uploaded and verified in GitHub.

---

## Documentation Security Review

Before final publication, verify that screenshots do not expose:

- Personal email addresses
- User principal names
- Tenant IDs
- Subscription IDs
- Object IDs
- Secrets, tokens, or keys
- Authentication details
- Billing information
- Unrelated browser tabs, bookmarks, or notifications containing sensitive information

The screenshots captured for this lab were reviewed during the lab workflow and did not require identified redactions at capture time. A final review will still be performed after repository upload.

---

## Outcome

The Microsoft Learn portion and MRTG knowledge-check portion of Lab 01 are complete. The lab demonstrates a working understanding of the foundational security, compliance, and identity concepts required before moving into Microsoft Entra configuration and analysis.

The remaining task is to upload the five sanitized screenshots and perform a final evidence review. After that, Lab 01 can be marked **Complete** and the root project progress can be updated to **1 of 12 labs complete**.

---

## Screenshot Inventory

```text
screenshots/
├── 00-sc900-course-starting-state.png
├── 01-shared-responsibility-model.png
├── 02-security-compliance-module-complete.png
├── 03-authentication-vs-authorization.png
└── 04-identity-concepts-and-learning-path-complete.png
```

---

## Screenshots

Screenshot links will be added after the sanitized image files are uploaded to the repository.

---

## Next Lab

```text
Lab 02 - Microsoft Entra Identity
```

Lab 02 will move from foundational identity concepts into practical exploration of Microsoft Entra ID, identity types, users, groups, roles, and the MRTG cloud identity environment.

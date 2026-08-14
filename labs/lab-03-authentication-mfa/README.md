# Lab 03 - Authentication and Multifactor Authentication

> **Status:** In Progress

## AI Use Disclosure

AI tools may be used to support learning, troubleshooting, documentation organization, and technical review during this lab. All hands-on work, validation, screenshots, administrative decisions, and final documentation review will be completed by the project author. AI-generated guidance will be reviewed against Microsoft documentation and observed lab results before being accepted.

---

## Lab Metadata

| Item | Value |
|---|---|
| Difficulty | Beginner |
| Estimated Time | 2-3 hours |
| Lab Type | Microsoft Learn + read-only discovery |
| SC-900 Domain | Describe the capabilities of Microsoft Entra |
| Primary Objective | Describe authentication capabilities of Microsoft Entra ID |
| Previous Lab Dependency | Lab 02 - Microsoft Entra Identity |
| Next Lab Dependency | Lab 04 - RBAC and Conditional Access |

---

## Objective

Build a practical understanding of Microsoft Entra ID authentication capabilities and explain how stronger authentication reduces the risk of account compromise.

This lab focuses on the Microsoft Learn module **Describe the authentication capabilities of Microsoft Entra ID** and covers:

- Authentication methods in Microsoft Entra ID
- Password-based authentication
- Passwordless authentication concepts
- Microsoft Authenticator
- Passkeys / FIDO2 concepts
- Windows Hello for Business concepts
- Multifactor authentication (MFA)
- Authentication factors
- Self-service password reset (SSPR)
- Password protection and password management capabilities
- The security value of phishing-resistant authentication methods

Conditional Access policy design, Microsoft Entra roles, and RBAC are intentionally deferred to Lab 04.

---

## Business Problem Solved

Monroe Redstone Technology Group (MRTG) needs to reduce the risk that a stolen or guessed password can be used to gain unauthorized access to organizational resources.

Without a strong authentication strategy, MRTG could experience:

- Account compromise from stolen passwords
- Password reuse and weak-password risk
- Phishing-based credential theft
- Excessive dependence on a single authentication factor
- Increased help desk workload from password-reset requests
- Inconsistent authentication-method usage
- Weak recovery processes for users who forget credentials
- Confusion between MFA, passwordless authentication, and access-control policies

---

## Scenario

MRTG is reviewing how users prove their identities before the organization designs more advanced access policies.

The security team must understand the available Microsoft Entra authentication methods, how MFA combines independent factors, how passwordless methods reduce dependence on passwords, how SSPR supports secure user recovery, and how Microsoft Entra password protection helps prevent weak or commonly attacked passwords.

The lab combines Microsoft Learn with sanitized read-only discovery in the Microsoft Entra admin center. No production authentication policy should be changed solely to create portfolio evidence.

---

## Success Criteria

The lab is successful when:

- The Microsoft Learn module **Describe the authentication capabilities of Microsoft Entra ID** is completed
- The module assessment is passed
- Authentication factors can be distinguished as something you know, have, or are
- Common Microsoft Entra authentication methods can be identified
- MFA can be explained as requiring multiple independent authentication factors
- Passwordless authentication can be distinguished from password + MFA
- Stronger and phishing-resistant authentication approaches can be recognized
- SSPR can be explained in practical IAM and help desk terms
- Password protection and password-management capabilities can be explained
- Authentication methods can be explored in the Microsoft Entra admin center without unnecessary configuration changes
- Screenshots are sanitized before publication

---

## Prerequisites

- Completed Lab 02
- Access to Microsoft Learn
- General Azure and Microsoft 365 fundamentals
- Access to the Microsoft Entra admin center for read-only discovery
- Access to the project GitHub repository

---

## Expected Starting State

- Lab 02 complete
- No Lab 03 authentication configuration changes performed
- Microsoft Learn **Introduction to Microsoft Entra** learning path available
- Microsoft Entra admin center available for discovery
- No requirement to use a personal identity for evidence

---

## Required Permissions

| Permission or Role | Purpose | Required |
|---|---|---|
| Microsoft Learn account | Complete module and assessment | Yes |
| Microsoft Entra tenant access | Read-only authentication discovery | Recommended |
| Privileged Entra role | Not required for core lab | No |

Use the least privilege available. Do not elevate permissions simply to capture screenshots.

---

## Services and Resources Used

| Service or Resource | Purpose |
|---|---|
| Microsoft Learn | SC-900 authentication training and assessment |
| Microsoft Entra admin center | Read-only authentication-method discovery |
| GitHub | Documentation and sanitized evidence storage |

---

## Why These Services Are Used

Microsoft Learn provides the official SC-900 training content. The Microsoft Entra admin center connects the authentication concepts to the administrative interface used by identity teams. GitHub provides a version-controlled portfolio record of the lab.

---

## Environment

```text
Organization: Monroe Redstone Technology Group (MRTG)
Lab mode: Microsoft Learn + read-only discovery
Azure consumption resources deployed: None
Authentication policy changes required: None
Estimated Azure consumption cost: $0.00
```

---

## Architecture / Concept Diagram

```text
Identity claims access
        |
        v
Authentication challenge
        |
        +--> Something you know
        |      Example: password / PIN
        |
        +--> Something you have
        |      Example: registered device / security key
        |
        +--> Something you are
               Example: biometric
        |
        v
Identity verified
        |
        v
Authorization / access decision
```

MFA requires authentication using more than one independent factor. Simply repeating the same factor category does not create true multifactor authentication.

---

## Lab Safety and Change Control

- Confirm the correct Microsoft Entra tenant before portal activity.
- Prefer read-only discovery for this lab.
- Do not disable or weaken authentication protections for testing.
- Do not enroll a personal phone number, personal email address, or personal biometric solely for portfolio evidence.
- Do not publish authentication-method details tied to a real user.
- Do not expose personal names, email addresses, UPNs, tenant IDs, object IDs, phone numbers, QR codes, secrets, tokens, recovery information, or authentication-session details.
- Avoid publishing unnecessary tenant security-posture details.
- Sanitize all screenshots before committing them to GitHub.
- Treat AI-generated guidance as secondary to Microsoft documentation and observed results.

---

## Microsoft Learn Content

### Learning Path

**Introduction to Microsoft Entra**

Lab 03 covers the module:

**Describe the authentication capabilities of Microsoft Entra ID**

### Current Module Learning Objectives

After completing the module, the learner should be able to:

- Describe the authentication methods of Microsoft Entra ID
- Describe multifactor authentication (MFA) in Microsoft Entra ID
- Describe self-service password reset (SSPR) in Microsoft Entra ID
- Describe the password protection and management capabilities of Microsoft Entra ID

### Module Units

1. Introduction
2. Describe authentication methods
3. Describe multifactor authentication
4. Describe self-service password reset
5. Describe password protection and management capabilities
6. Module assessment
7. Summary and resources

---

## Discovery Activities

Where tenant access is available, perform sanitized read-only exploration of authentication-related areas in the Microsoft Entra admin center.

Possible discovery targets include:

1. Microsoft Entra ID authentication methods
2. Authentication methods policy overview
3. Password reset / SSPR settings where available
4. Password protection settings where available

Do not change method enablement, user targeting, registration settings, or password-reset configuration solely for portfolio evidence.

---

## Concept Work to Produce

The completed Lab 03 documentation will include:

1. **Authentication Factor Matrix** - know, have, and are
2. **Authentication Method Comparison** - password, Authenticator, passkeys/FIDO2, Windows Hello for Business, certificate-based authentication, Temporary Access Pass, and other methods at an SC-900 level
3. **MFA Summary** - why multiple independent factors improve security
4. **Passwordless vs. MFA Comparison** - why passwordless does not simply mean "no security"
5. **Phishing-Resistance Note** - distinguish stronger phishing-resistant methods from methods that remain vulnerable to remote phishing
6. **SSPR Summary** - secure user-driven password recovery and help desk impact
7. **Password Protection Summary** - banned-password concepts and password-management protections

---

## Planned Evidence

Keep the screenshot set small and useful:

| Screenshot | Evidence |
|---|---|
| `00-entra-authentication-module-starting-state.png` | Microsoft Learn authentication module starting state and objectives |
| `01-entra-authentication-methods.png` | Strong Microsoft Learn visual or sanitized Entra authentication-methods discovery |
| `02-entra-multifactor-authentication.png` | MFA concept evidence |
| `03-entra-sspr-or-password-protection.png` | Strong SSPR or password-protection evidence; choose the better visual rather than capturing both without need |
| `04-entra-authentication-module-complete.png` | Passed module assessment and module completion |

Only screenshots actually captured and sanitized will remain in the final README.

---

## Supporting Concept Summary

To be completed after Microsoft Learn review and scenario-based knowledge checks.

---

## Evidence Collected

To be completed after sanitized evidence is captured and uploaded.

---

## Validation

Validation will be performed through:

- Microsoft Learn module assessment
- Scenario-based authentication-method knowledge checks
- MFA factor-identification exercises
- Passwordless vs. password + MFA comparison
- SSPR scenario review
- Password-protection scenario review
- Repository evidence verification

---

## Completion Checklist

- [ ] Capture starting-state screenshot
- [ ] Complete authentication methods section
- [ ] Complete MFA section
- [ ] Complete SSPR section
- [ ] Complete password protection and management section
- [ ] Pass module assessment
- [ ] Perform sanitized Entra authentication discovery
- [ ] Complete authentication-factor knowledge check
- [ ] Complete authentication-method knowledge check
- [ ] Complete MFA knowledge check
- [ ] Complete passwordless knowledge check
- [ ] Complete SSPR knowledge check
- [ ] Complete password-protection knowledge check
- [ ] Upload sanitized screenshots
- [ ] Perform final repository evidence review
- [ ] Mark Lab 03 complete

---

## SC-900 Exam Objective Coverage

### Primary Exam Domain

```text
Describe the capabilities of Microsoft Entra
```

### Primary Skill Area

```text
Describe authentication capabilities of Microsoft Entra ID
```

The current SC-900 skills measured include:

- Describe the authentication methods
- Describe multifactor authentication (MFA)
- Describe password protection and management capabilities

SSPR is included in the Microsoft Learn authentication module and is treated in this lab as a supporting authentication and recovery concept.

---

## Mini Objective Coverage

To be completed after validation.

---

## Exam Traps and Key Distinctions

Initial distinctions to validate during the lab:

- Authentication is not authorization.
- MFA requires more than one independent factor category.
- Two passwords do not equal MFA because both are "something you know."
- Passwordless authentication does not mean authentication is removed; it replaces the password with stronger authentication mechanisms.
- A managed or registered authentication method is not necessarily required for every sign-in unless an applicable policy requires it.
- SSPR is an account-recovery/password-reset capability, not an authorization system.
- Stronger authentication does not replace least privilege or access-control policy.

---

## IAM / Security Relevance

Authentication is one of the most practical IAM responsibilities because it answers:

```text
Can this identity prove that it is who it claims to be?
```

Identity administrators must balance usability, recovery, phishing resistance, account security, and operational support when selecting and governing authentication methods.

---

## On-Premises Connection

Traditional AD DS environments commonly rely on passwords and may use additional authentication products or smart cards. Hybrid identity environments can extend Microsoft Entra authentication and recovery capabilities to cloud-connected users while still requiring careful design around on-premises password and identity infrastructure.

---

## Security Analysis

This lab will evaluate authentication risk from the perspective that a password can be guessed, reused, phished, leaked, or stolen. Strong authentication should reduce dependence on a single shared secret and make successful account takeover more difficult.

---

## Zero Trust Analysis

Authentication directly supports **verify explicitly**.

MRTG should verify identities using the strongest practical authentication signals and should not assume that possession of a password alone proves a user is trustworthy.

Authentication must still be combined with:

- Least privilege
- Appropriate access policies
- Device and risk signals where applicable
- Monitoring
- An assumption that credentials or sessions can be compromised

---

## Governance and Compliance Notes

Authentication-method governance should define which methods are permitted, who can use them, how users register and recover authentication methods, and how high-risk or privileged identities receive stronger protections.

---

## Cost and Licensing Considerations

```text
Estimated Azure consumption cost: $0.00
```

The core lab uses Microsoft Learn and read-only Microsoft Entra discovery. No Azure consumption resources are required.

Authentication capabilities and enforcement options can have licensing, tenant, and policy dependencies. Any premium requirement encountered during hands-on discovery will be documented rather than bypassed solely to complete the lab.

---

## Troubleshooting

To be completed if issues occur during the lab.

---

## What I Would Do Differently in Production

To be completed after the lab. Production recommendations should favor phishing-resistant authentication, least privilege, controlled registration and recovery, staged deployment, monitoring, and documented break-glass procedures where appropriate.

---

## Lessons Learned

To be completed after knowledge checks and validation.

---

## Skills Demonstrated

Planned skills include:

- Microsoft Entra authentication fundamentals
- MFA concepts
- Authentication-method analysis
- Passwordless authentication concepts
- SSPR concepts
- Password protection concepts
- Identity security analysis
- Zero Trust authentication reasoning
- Read-only Entra administrative discovery
- Security-conscious evidence collection

---

## Cleanup

No Azure consumption resources or authentication-policy changes are planned for the core lab, so no technical cleanup should be required.

Any temporary evidence files outside the repository should be deleted after sanitized versions are committed.

---

## Documentation Security Review

Before completion, verify that screenshots and documentation do not expose:

- Personal email addresses or UPNs
- Phone numbers
- Tenant IDs or object IDs
- Authentication QR codes
- Temporary Access Pass values
- Recovery information
- Secrets or tokens
- Authentication-session details
- User-specific authentication methods
- Unnecessary security-posture information

---

## Screenshot Inventory

To be completed after final evidence selection.

---

## Next Lab

```text
Lab 04 - RBAC and Conditional Access
```

Lab 04 will continue the Microsoft Entra learning path with access management, Conditional Access, Microsoft Entra roles, and role-based access control concepts.

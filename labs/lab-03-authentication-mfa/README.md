# Lab 03 - Authentication and Multifactor Authentication

> **Status:** Complete

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

This lab focused on the Microsoft Learn module **Describe the authentication capabilities of Microsoft Entra ID** and covered:

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

The lab combined Microsoft Learn with sanitized read-only discovery in the Microsoft Entra admin center. No production authentication policy changes were made solely to create portfolio evidence.

---

## Success Criteria

The lab was successful because:

- The Microsoft Learn module **Describe the authentication capabilities of Microsoft Entra ID** was completed
- The module assessment was passed
- Authentication factors were distinguished as something you know, have, or are
- Common Microsoft Entra authentication methods were identified
- MFA was explained as requiring multiple independent authentication factors
- Passwordless authentication was distinguished from password + MFA
- Stronger and phishing-resistant authentication approaches were recognized
- SSPR was explained in practical IAM and help desk terms
- Password protection and password-management capabilities were reviewed
- Authentication-related areas were explored in the Microsoft Entra admin center without unnecessary configuration changes
- Screenshots were reviewed and sanitized before publication

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

Least privilege was maintained. No privilege elevation was required solely for screenshot capture or exploration.

---

## Services and Resources Used

| Service or Resource | Purpose |
|---|---|
| Microsoft Learn | SC-900 authentication training and assessment |
| Microsoft Entra admin center | Read-only authentication-method discovery |
| GitHub | Documentation and sanitized evidence storage |

---

## Why These Services Are Used

Microsoft Learn provides the official SC-900 training content. The Microsoft Entra admin center connects authentication concepts to the administrative interface used by identity teams. GitHub provides a version-controlled portfolio record of the lab.

---

## Environment

```text
Organization: Monroe Redstone Technology Group (MRTG)
Lab mode: Microsoft Learn + read-only discovery
Azure consumption resources deployed: None
Authentication policy changes performed: None
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

- Confirmed the correct Microsoft Entra tenant before portal activity.
- Used read-only discovery for the administrative portion of the lab.
- Did not disable or weaken authentication protections for testing.
- Did not enroll a personal phone number, personal email address, or personal biometric solely for portfolio evidence.
- Did not publish authentication-method details tied to a real user.
- Avoided exposing personal names, email addresses, UPNs, tenant IDs, object IDs, phone numbers, QR codes, secrets, tokens, recovery information, or authentication-session details.
- Avoided publishing unnecessary tenant security-posture details.
- Reviewed screenshots before committing them to GitHub.
- Treated AI-generated guidance as secondary to Microsoft documentation and observed results.

---

## Steps Performed

1. Opened the Microsoft Learn module **Describe the authentication capabilities of Microsoft Entra ID**.
2. Reviewed Microsoft Entra authentication methods and their use for primary authentication, MFA, SSPR, and account recovery.
3. Reviewed the three common authentication-factor categories: something you know, something you have, and something you are.
4. Reviewed multifactor authentication and the requirement to combine independent factor categories.
5. Compared password-based, passwordless, and phishing-resistant authentication approaches.
6. Reviewed Microsoft Authenticator, passkeys/FIDO2, Windows Hello for Business, certificate-based authentication, Temporary Access Pass, OATH, SMS, voice, and related methods at an SC-900 level.
7. Reviewed SSPR and the distinction between normal password reset and broader account recovery scenarios.
8. Reviewed password protection and password-management concepts.
9. Passed the Microsoft Learn module assessment.
10. Performed scenario-based knowledge checks covering authentication factors, MFA, passwordless authentication, SSPR, password protection, and phishing-resistant authentication.
11. Performed read-only discovery in the Microsoft Entra admin center, including:
    - Entra ID > Authentication methods > Policies
    - Entra ID > Password reset
    - Entra ID > Authentication methods > Password protection
12. Uploaded and verified the final sanitized screenshot set in GitHub.

---

## Microsoft Learn Content

### Learning Path

**Introduction to Microsoft Entra**

Lab 03 covered the module:

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

## Supporting Concept Summary

### Authentication Factor Matrix

| Factor Category | Meaning | Examples |
|---|---|---|
| Something you know | A secret known by the user | Password, PIN |
| Something you have | A physical or registered possession | Security key, registered phone, authenticator device |
| Something you are | A biometric characteristic | Fingerprint, facial recognition |

A second prompt does not automatically create MFA. For example, a password plus another knowledge-based secret remains within the same factor category.

### Authentication Method Comparison

| Method | SC-900-Level Security Purpose |
|---|---|
| Password | Common primary credential but vulnerable to guessing, reuse, leakage, and phishing |
| Microsoft Authenticator | Supports passwordless sign-in and MFA depending on configuration and use |
| Passkeys / FIDO2 | Strong passwordless authentication and an important phishing-resistant direction |
| Windows Hello for Business | Uses device-bound credentials with a local gesture such as a PIN or biometric |
| Certificate-based authentication | Uses certificates as strong credentials in supported deployments |
| Temporary Access Pass | Time-limited credential commonly used to bootstrap or recover registration for stronger methods |
| OATH tokens | Can provide one-time passcodes for secondary authentication |
| SMS / voice | Can support MFA or recovery but provide weaker resistance to phishing and social engineering than phishing-resistant methods |

### MFA Summary

MFA improves account security by requiring more than one independent factor category. A stolen password alone should not be sufficient to authenticate when a properly designed MFA requirement is enforced.

### Passwordless vs. MFA

Passwordless authentication removes the password from the sign-in process and replaces it with another credential mechanism. It does not mean authentication is removed. Some passwordless methods can provide multifactor characteristics through a combination such as device possession plus a local biometric or PIN gesture.

### Phishing Resistance

Passkeys/FIDO2 and Windows Hello for Business represent stronger phishing-resistant directions because the credential is designed to avoid exposing a reusable password or remotely phishable shared secret. SMS and voice can still support MFA but are not equivalent to phishing-resistant credentials.

### SSPR

Self-service password reset allows users who still have access to approved registered verification methods to reset a forgotten password without requiring a help desk technician to perform the reset manually.

This reduces support workload while preserving identity verification requirements.

The Learn content also distinguishes broader account recovery scenarios in which a user has lost access to all authentication methods and requires a more comprehensive recovery process.

### Password Protection

Microsoft Entra password protection helps prevent weak and commonly attacked passwords by identifying banned-password patterns and reducing the likelihood that predictable credentials are accepted.

---

## Evidence Collected

| Screenshot | Evidence |
|---|---|
| `00-entra-authentication-module-starting-state.png` | Microsoft Learn authentication module starting state and learning objectives |
| `01-entra-authentication-methods.png` | Current authentication-method comparison showing primary and secondary authentication uses |
| `02-entra-multifactor-authentication.png` | Conceptual MFA flow showing independent authentication factors and Microsoft Entra ID as verifier |
| `03-entra-sspr-or-password-protection.png` | Comparison of self-service password reset and broader account recovery |
| `04-entra-authentication-module-complete.png` | Module assessment passed and module completion |

---

## Validation

| Validation Activity | Result |
|---|---|
| Microsoft Learn module completed | Passed |
| Microsoft Learn module assessment | Passed |
| Authentication factor identification | Passed |
| MFA knowledge check | Passed |
| Passwordless authentication knowledge check | Passed |
| SSPR knowledge check | Passed |
| Password protection knowledge check | Passed |
| Phishing-resistant authentication scenario | Passed |
| Microsoft Entra read-only discovery | Completed |
| Repository screenshot verification | Completed |

Knowledge-check examples validated that:

- Password is something you know.
- A security key is something you have.
- A fingerprint is something you are.
- A registered Authenticator device is something you have.
- A PIN is something you know.
- Password + security key is MFA because the two methods represent different factor categories.
- Passwordless authentication replaces the password rather than eliminating authentication.
- SSPR is appropriate when a user forgets a password but still has access to registered verification methods.
- Microsoft Entra password protection addresses weak and commonly attacked passwords.
- Passkeys/FIDO2 are a stronger phishing-resistant direction than password-only or SMS-based authentication.

---

## Completion Checklist

- [x] Capture starting-state screenshot
- [x] Complete authentication methods section
- [x] Complete MFA section
- [x] Complete SSPR section
- [x] Complete password protection and management section
- [x] Pass module assessment
- [x] Perform sanitized Entra authentication discovery
- [x] Complete authentication-factor knowledge check
- [x] Complete authentication-method knowledge check
- [x] Complete MFA knowledge check
- [x] Complete passwordless knowledge check
- [x] Complete SSPR knowledge check
- [x] Complete password-protection knowledge check
- [x] Upload sanitized screenshots
- [x] Perform final repository evidence review
- [x] Mark Lab 03 complete

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

The SC-900 skills covered by this lab include:

- Describe authentication methods
- Describe multifactor authentication (MFA)
- Describe password protection and management capabilities

SSPR is included in the Microsoft Learn authentication module and is treated in this lab as a supporting authentication and recovery concept.

---

## Mini Objective Coverage

| Objective | Coverage |
|---|---|
| Authentication methods | Reviewed Microsoft Entra methods and compared their primary, secondary, passwordless, and recovery uses |
| Multifactor authentication | Identified factor categories and validated what does and does not qualify as MFA |
| Passwordless authentication | Distinguished passwordless authentication from password + MFA and from unauthenticated access |
| Phishing-resistant authentication | Identified passkeys/FIDO2 and Windows Hello for Business as stronger authentication directions |
| SSPR | Explained self-service password reset and its help desk / IAM value |
| Password protection | Reviewed weak-password and banned-password protection concepts |
| Administrative discovery | Reviewed authentication methods, SSPR, and password protection areas in Microsoft Entra without making changes |

---

## Exam Traps and Key Distinctions

- Authentication is not authorization.
- MFA requires more than one independent factor category.
- Two passwords do not equal MFA because both are something you know.
- A password plus a security key can provide MFA because it combines something you know with something you have.
- Passwordless authentication does not mean authentication is removed; it replaces the password with another credential mechanism.
- Passwordless and MFA are related but are not identical concepts.
- SSPR is a password-recovery capability, not an authorization system.
- Temporary Access Pass is intended as a temporary credential and is not a normal long-term replacement for strong authentication methods.
- SMS and voice can support MFA but are not equivalent to phishing-resistant authentication.
- Strong authentication does not replace least privilege, Conditional Access, RBAC, monitoring, or other access controls.

---

## IAM / Security Relevance

Authentication is one of the most practical IAM responsibilities because it answers:

```text
Can this identity prove that it is who it claims to be?
```

Identity administrators must balance usability, recovery, phishing resistance, account security, and operational support when selecting and governing authentication methods.

This lab also reinforces a common IAM support boundary: restoring authentication is not the same as granting authorization. A user can successfully authenticate and still lack permission to a resource.

---

## On-Premises Connection

Traditional AD DS environments commonly rely on passwords and may use additional authentication products or smart cards. Hybrid identity environments can extend Microsoft Entra authentication and recovery capabilities to cloud-connected users while still requiring careful design around on-premises password and identity infrastructure.

Password protection can also be relevant to hybrid environments where organizations want stronger password controls to extend beyond cloud-only identities.

---

## Security Analysis

Passwords can be guessed, reused, phished, leaked, or stolen. Authentication design should therefore reduce dependence on a single reusable secret.

MRTG's strongest direction is to:

- Prefer phishing-resistant authentication for privileged and high-risk identities
- Use MFA where passwordless or phishing-resistant methods are not yet practical
- Restrict weak or legacy authentication choices where possible
- Govern method registration and recovery carefully
- Protect the recovery process with the same seriousness as the primary sign-in process
- Monitor authentication activity for suspicious behavior

A strong primary authentication method is valuable, but compromised sessions, misconfigured permissions, or overly broad authorization can still create risk after sign-in.

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

Authentication-method governance should define:

- Which methods are permitted
- Which identity populations may use each method
- How users register methods
- How users recover access
- How privileged and high-risk identities receive stronger protections
- How authentication changes are documented and monitored

In regulated environments, authentication and recovery procedures should also support auditable identity verification and consistent policy enforcement.

---

## Cost and Licensing Considerations

```text
Estimated Azure consumption cost: $0.00
```

The core lab used Microsoft Learn and read-only Microsoft Entra discovery. No Azure consumption resources were deployed.

Authentication capabilities and enforcement options can have licensing, tenant, and policy dependencies. Premium requirements should be documented rather than bypassed solely to complete a lab.

---

## Troubleshooting

No material technical issues were encountered during the core lab.

The primary constraint was keeping the evidence set useful while avoiding user-specific authentication data and unnecessary tenant security details. The solution was to rely primarily on Microsoft Learn evidence and use the Entra admin center for read-only discovery without publishing sensitive portal views.

---

## What I Would Do Differently in Production

In a production rollout, MRTG should not enable authentication changes broadly without planning and staged validation.

A stronger production approach would include:

- Inventory current authentication-method usage
- Identify privileged and high-risk populations first
- Establish emergency-access / break-glass procedures
- Pilot stronger methods with a controlled user group
- Prefer phishing-resistant methods where practical
- Define approved registration and recovery processes
- Communicate user-impact changes before enforcement
- Monitor sign-in and registration activity
- Document rollback and support procedures
- Apply Conditional Access and authorization controls separately from authentication-method configuration

---

## Lessons Learned

- Authentication proves identity; authorization determines what that identity may access.
- MFA depends on independent factor categories, not simply multiple prompts.
- Passwordless authentication still requires strong identity verification.
- Phishing-resistant authentication provides a stronger security direction than reusable passwords or remotely phishable codes.
- SSPR can reduce help desk workload while preserving identity verification.
- Recovery methods are part of the authentication security boundary and must be governed carefully.
- Authentication-method choice should be based on risk, usability, recovery, and operational requirements rather than convenience alone.
- Read-only administrative discovery is often enough to connect certification concepts to real portal workflows without changing tenant configuration.

---

## Skills Demonstrated

- Microsoft Entra authentication fundamentals
- Authentication-factor classification
- MFA concepts and validation
- Authentication-method analysis
- Passwordless authentication concepts
- Passkey/FIDO2 concepts
- Windows Hello for Business concepts
- SSPR concepts
- Password protection concepts
- Phishing-resistance analysis
- Identity security analysis
- Zero Trust authentication reasoning
- Read-only Entra administrative discovery
- Security-conscious evidence collection
- Scenario-based SC-900 knowledge validation

---

## Cleanup

No Azure consumption resources or authentication-policy changes were created during the core lab, so no technical cleanup was required.

Temporary evidence files outside the repository should be removed after sanitized versions are committed.

---

## Documentation Security Review

Final review confirmed that the published screenshot set does not intentionally expose:

- Personal email addresses or UPNs
- Phone numbers
- Tenant IDs or object IDs
- Authentication QR codes
- Temporary Access Pass values
- Recovery information
- Secrets or tokens
- Authentication-session details
- User-specific authentication methods
- Unnecessary tenant security-posture information

The final evidence set was intentionally kept small and concept-focused.

---

## Screenshot Inventory

| Screenshot | Status | Purpose |
|---|---|---|
| `00-entra-authentication-module-starting-state.png` | Included | Starting state and module objectives |
| `01-entra-authentication-methods.png` | Included | Authentication-method comparison |
| `02-entra-multifactor-authentication.png` | Included | MFA and independent-factor concept |
| `03-entra-sspr-or-password-protection.png` | Included | SSPR vs. broader account recovery |
| `04-entra-authentication-module-complete.png` | Included | Passed assessment and module completion |

---

## Outcome

Lab 03 successfully established the authentication foundation needed for later Microsoft Entra access-control work.

MRTG can now distinguish authentication factors, explain MFA, compare password and passwordless methods, identify stronger phishing-resistant authentication approaches, explain SSPR and password protection, and recognize the administrative areas in Microsoft Entra where these capabilities are governed.

**Lab 03 status: Complete.**

---

## Next Lab

```text
Lab 04 - RBAC and Conditional Access
```

Lab 04 will continue the Microsoft Entra learning path with access management, Conditional Access, Microsoft Entra roles, and role-based access control concepts.

# Login and Access Issue Troubleshooting

Use this guide for sign-in failures and requests to access a resource. Authentication confirms identity; authorization determines what that identity may do. A successful sign-in does not by itself prove that access is correctly assigned.

## Symptoms

- Credentials are rejected or sign-in repeatedly redirects or prompts for multifactor authentication (MFA).
- An account is locked, disabled, or reported as expired.
- Sign-in succeeds, but a particular application, group, or file returns access denied.
- A new device or changed network triggers an additional identity check.

## Investigation

1. Confirm the user through the approved identity-verification process before discussing or changing account details. Never request a password or MFA code.
2. Capture the exact message, time, application/resource, device, sign-in method, and whether other services work. Obtain a request/correlation ID if shown.
3. Distinguish authentication failure from authorization failure. Check account status and sign-in logs only if the role permits; note whether MFA was completed and whether the event is expected.
4. Check the approved identity or service status source, and compare with a known-good service without asking the user to share secrets.
5. For access denied, confirm the requested resource and business need, current role/group assignment through an authorized source, and whether an approval is required. Do not grant access based solely on a verbal request.
6. Consider recent password, MFA device, role, employment-status, policy, or application changes. Do not weaken MFA or conditional-access controls to restore access.

## Possible causes

- Typing/layout issue, stale saved credential, expired password, lockout, or disabled account.
- MFA enrollment/device issue, time mismatch, or identity-provider/service disruption.
- Missing or stale role/group assignment, wrong account, or resource-specific permission.
- Conditional-access policy, untrusted device/network, or session/cookie issue.
- Provisioning delay or recent identity/application change.

## Resolution and verification

- Follow approved self-service reset, unlock, or MFA recovery procedures after identity verification. Do not collect or transmit passwords, recovery codes, or MFA tokens.
- Route access changes through the designated approval and provisioning process. Apply only permissions that are approved and within the support role.
- Have the user sign in and verify the specific requested resource and expected level of access. Record the approval reference, action, and outcome without storing secrets.

## Escalate when

- The user cannot be safely verified, there are repeated unexpected MFA prompts, suspicious sign-ins, or possible account compromise.
- Multiple users are affected or identity-provider services appear unavailable.
- Account status, entitlements, or audit evidence conflict, or privileged access is requested.
- The requested grant lacks required approval or exceeds the support role.

Preserve relevant timestamps and correlation IDs and use the security or identity escalation route where applicable. Avoid including passwords, tokens, recovery codes, or unnecessary personal information in tickets.

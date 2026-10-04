# Stark Industries IAM Security Lab — Project Tracker

## Project Goal

Build and validate a small Microsoft Entra ID IAM security environment demonstrating:

**Provision → Authenticate → Authorize → Monitor → Modify → Revoke → Validate**

The project focuses specifically on identity security, least privilege, authentication controls, privileged access, identity monitoring, and lifecycle management.

---

## Lab Environment

### Infrastructure
- WATCHTOWER — Windows 11 physical Hyper-V host
- STARK-3725 — Windows 11 Pro VM
  - Microsoft Entra joined
  - Intune managed
  - Windows Autopilot registered

### Microsoft Cloud
- Microsoft Entra ID
- Microsoft Entra ID P2
- Microsoft Intune

---

## IAM Architecture

### Identities
- Tony Stark (`tstark`) — existing test identity
- Pepper Potts — business/executive identity
- Happy Hogan — Joiner / Mover / Leaver lifecycle identity
- Dedicated IAM Administrator — privileged identity
- Existing Global Administrator — tenant/bootstrap administration only

### Security Groups
- `SG-Executive`
- `SG-Security`
- `SG-Operations`

---

# Phase 1 — Identity Foundation

- [x] Review existing Stark Industries Entra users, groups, and policies before making changes
- [x] Create required IAM lab identities
- [x] Create the three IAM security groups
- [x] Assign initial group memberships based on job requirements
- [x] Validate initial user and group configuration
- [x] Capture purposeful evidence of the identity/access model

---

# Phase 2 — Authentication Security

- [x] Review authentication methods available in the tenant
- [x] Configure/test MFA for the selected lab identity
- [x] Create one targeted Conditional Access policy
- [x] Test expected authentication behavior
- [x] Validate successful and blocked/challenged authentication behavior
- [x] Document the security purpose of the authentication controls

---

# Phase 3 — Least Privilege and Privileged Access

- [x] Configure the dedicated IAM Administrator identity
- [x] Select one appropriate limited administrative role
- [x] Configure the role through Privileged Identity Management (PIM)
- [x] Activate the eligible role
- [x] Perform and validate one privileged administrative action
- [x] Validate removal/expiration of elevated privileges
- [x] Document permanent privilege vs. just-in-time privilege

---

# Phase 4 — Joiner / Mover Security Scenario

- [ ] Provision Happy Hogan as an Operations employee
- [ ] Validate `SG-Operations` access
- [ ] Simulate Happy moving to a security-related role
- [ ] Grant required `SG-Security` access
- [ ] Intentionally leave stale `SG-Operations` membership
- [ ] Identify the excessive/stale authorization
- [ ] Remove inappropriate access
- [ ] Validate Happy's corrected least-privilege access

---

# Phase 5 — Identity Monitoring and Investigation

- [ ] Generate controlled authentication activity
- [ ] Review Microsoft Entra sign-in logs
- [ ] Review Microsoft Entra audit logs
- [ ] Review relevant Identity Protection information
- [ ] Investigate one authentication or identity-related event
- [ ] Document evidence, findings, and remediation where applicable

---

# Phase 6 — Leaver / Access Revocation

- [ ] Simulate Happy Hogan leaving Stark Industries
- [ ] Disable Happy's account
- [ ] Remove authorization/group access
- [ ] Revoke existing sessions where appropriate
- [ ] Attempt authentication/access after termination
- [ ] Validate that former access is no longer available
- [ ] Document the complete Joiner → Mover → Leaver lifecycle

---

# Phase 7 — Documentation and Portfolio Completion

- [ ] Create final IAM architecture / identity-flow diagram
- [ ] Organize purposeful screenshots
- [ ] Add any small PowerShell scripts used during the project
- [ ] Document IAM security scenarios and troubleshooting
- [ ] Document validation results
- [ ] Write lessons learned
- [ ] Complete README
- [ ] Create conservative resume bullets based only on completed work
- [ ] Verify all technical claims against actual lab evidence
- [ ] Perform final GitHub repository cleanup
- [ ] Make repository public when ready for portfolio use

---

## Scope Guardrails

- Keep the project focused on IAM security.
- Do not expand into general Microsoft 365 administration.
- Do not rebuild Active Directory infrastructure.
- Do not expand Intune configuration unless required for IAM validation.
- Do not add additional VMs unless technically necessary.
- Do not add additional identities or groups without a clear IAM requirement.
- Use PowerShell only when it adds meaningful IAM/security value.
- Use Microsoft Graph only if it provides substantial value that cannot be demonstrated more efficiently.
- Access Reviews and Entitlement Management are outside the planned scope.
- Lab experience must always be identified as lab experience.
- Do not claim professional experience from work performed in this project.

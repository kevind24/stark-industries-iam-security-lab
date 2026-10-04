# Stark Industries IAM Security Lab

## Overview

This project is a hands-on Identity and Access Management (IAM) security lab built in Microsoft Entra ID.

The lab focuses on implementing and validating a realistic identity lifecycle:

**Provision → Authenticate → Authorize → Monitor → Modify → Revoke → Validate**

The project is intentionally small and focuses on identity security concepts rather than general Microsoft 365 or endpoint administration.

## Objectives

- Implement identity lifecycle management
- Apply role-based access and least-privilege principles
- Configure and test multifactor authentication
- Implement a targeted Conditional Access control
- Demonstrate privileged access using Microsoft Entra Privileged Identity Management (PIM)
- Monitor identity activity using sign-in and audit logs
- Investigate identity-related security events
- Identify and remediate stale or excessive access
- Perform and validate account access revocation

## Environment

### Microsoft Cloud
- Microsoft Entra ID
- Microsoft Entra ID P2
- Microsoft Intune

### Endpoint
- `STARK-3725` — Windows 11 Pro
  - Microsoft Entra joined
  - Microsoft Intune managed
  - Windows Autopilot registered

### Host
- `WATCHTOWER` — Windows 11 Hyper-V host

## IAM Scenario

The lab uses a fictional Stark Industries environment with a deliberately small identity population.

The primary lifecycle scenario follows Happy Hogan through a **Joiner → Mover → Leaver** workflow. The project will validate how access is granted based on job requirements, modified when responsibilities change, monitored for inappropriate authorization, and revoked when employment ends.

A separate privileged identity will be used to demonstrate least-privilege administrative access and Privileged Identity Management.

## Project Status

**Status:** In Progress

See [`PROJECT-TRACKER.md`](PROJECT-TRACKER.md) for the current implementation status and project scope.

## Documentation

Implementation details, security scenarios, screenshots, validation results, and lessons learned will be added as the lab is completed.

> This repository documents hands-on lab experience in a controlled environment. It does not represent production implementation or professional enterprise IAM administration experience.

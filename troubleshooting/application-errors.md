# Application Error Troubleshooting

This guide covers an application that fails to start, crashes, returns an error, or behaves differently from expected. Protect user data and avoid repeating actions that could submit a transaction more than once.

## Symptoms

- An application will not launch or closes unexpectedly.
- A user sees an error code, blank page, failed request, or repeated timeout.
- A feature fails for one user, one device, or many users.
- A recent update appears to correlate with a change in behavior.

## Investigation

1. Capture the exact error text/code, time, application and version, device/OS, user impact, and the steps that reproduce it. Ask whether unsaved work or a transaction is at risk.
2. Determine scope: one session, one user, one device, one site, or multiple users. Check the approved service status or monitoring source if available.
3. Reproduce with a safe, non-production action where possible. Record the shortest reliable sequence and expected versus actual behavior.
4. Check relevant basics: connectivity, service dependencies, available disk space, supported version, and whether the issue follows the user or the device. Review application logs only through approved tools and redact secrets or personal data.
5. Compare with a known-good user/device or supported browser profile. Note recent deployments, configuration changes, or updates without assuming causation.
6. Before clearing caches, resetting profiles, reinstalling, or retrying a submission, consider data loss, session impact, and duplicate processing. Obtain the appropriate authorization.

## Possible causes

- Service-side outage, overload, or unavailable dependency.
- Client defect, incompatible version, corrupted local cache, or insufficient resources.
- Network, proxy, certificate, or DNS problem.
- User-specific settings, permissions, or stale session.
- Recent code, configuration, or data change.

## Resolution and verification

- Apply only a documented, approved workaround or repair that fits the support role. Preserve logs and user data before resetting local state.
- For a suspected service-side defect, provide the reproduction details and diagnostic evidence to the application owner rather than making unapproved production changes.
- Verify the original function with a safe test, confirm no duplicate transaction or lost work, and ask the requester to confirm recovery. Record any workaround and its limitations.

## Escalate when

- Multiple users or a business-critical workflow are affected, or the error suggests data loss, corruption, or a security issue.
- The issue began after a deployment or configuration change and rollback/change authority is needed.
- Resolution requires application-owner access, code changes, database work, or privileged administration.
- The problem persists after safe checks or lacks a known support procedure.

For escalation, include the error, timestamps/time zone, scope, application version, reproduction steps, expected/actual results, relevant sanitized logs or request IDs, and actions already taken.

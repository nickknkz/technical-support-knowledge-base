# Incident Escalation Process

Escalate when the issue exceeds the current team’s authority, access, expertise, or ability to contain impact. A good escalation transfers context and ownership clearly; it does not replace ongoing communication with the requester.

## When to escalate

- Impact is broad, increasing, time-critical, or affects a critical service.
- There is a suspected security event, safety concern, data loss, or integrity issue.
- Required access, change approval, specialist knowledge, or vendor action is outside the current role.
- Documented safe troubleshooting has not resolved the issue, or further action could cause harm.
- A service owner or incident coordinator needs to manage dependencies and communications.

Follow the organization’s incident and security channels, severity definitions, and on-call routing where established. For a suspected security event, preserve evidence and use the designated security path; do not investigate beyond authorization or alert a potentially involved party through an unapproved channel.

## Prepare the handoff

Include:

- Incident/ticket identifier, concise title, current owner, and best contact path.
- Service, business impact, scope, start time and latest update (include time zone).
- Current severity/priority and the facts supporting them; label estimates as estimates.
- Symptoms, exact errors, safe reproduction steps, and expected versus actual behavior.
- Checks performed and results, including what has not yet been checked.
- Relevant sanitized logs, correlation IDs, monitoring references, and recent changes.
- Workaround, risks, approvals obtained, and any action that must not be repeated.
- The specific help requested and the next update or review time.

Do not include passwords, MFA codes, access tokens, or unnecessary personal or confidential data. Use approved secure channels for restricted evidence.

## Handoff and follow-through

1. Contact the appropriate next-level team using the documented route. For urgent impact, use the urgent channel as well as the ticket if the process requires both.
2. State whether ownership is being transferred or specialist support is being requested while the current owner retains the ticket. Agree on the next owner and action explicitly.
3. Keep the ticket current, notify affected users of known facts and the next update point, and avoid promising a resolution time without confirmation.
4. If no acknowledgment arrives within the applicable local response target, use the next escalation route. Do not invent a target where none exists.
5. Reassess impact and priority as evidence changes. Record decisions and recovery verification.

## Fictional example

Several users at a remote office cannot reach an internal order service, while other sites can. The support analyst records affected users, locations, times, VPN state, and sanitized connectivity checks, then routes the incident to the network/service owners. The ticket identifies whether the analyst retains coordination and sets a next update point. Once the service is reachable, affected users verify the order workflow and the incident record captures the recovery evidence.

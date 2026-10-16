# Incident Prioritization

Prioritization helps a support team decide what to work on first and what response coordination is needed. Use the organization’s approved definitions and service targets where they exist; the model below is a practical starting point, not a company policy.

## Severity and priority

- **Severity** describes the incident’s impact: how much service is affected, how many users or processes are affected, and the consequences (including safety, security, data integrity, or regulatory impact).
- **Priority** describes the order and urgency of response. It is informed by severity, time sensitivity, available workarounds, and dependencies or deadlines.

They are related but not interchangeable. A severe incident generally merits urgent attention, while a lower-impact issue can still become time-critical if a deadline or dependency is imminent. Do not lower a severity rating just because a workaround exists; record the workaround and reassess overall impact.

## Assessment checklist

- [ ] What service, capability, or business process is affected?
- [ ] How many users, locations, or customers are affected? Is scope expanding?
- [ ] Is the service unavailable, degraded, or producing incorrect results?
- [ ] Is there a safe workaround, and how much effort or risk does it impose?
- [ ] Is there data loss/corruption, a security concern, or safety impact?
- [ ] Are there time-sensitive operations, external commitments, or dependencies?
- [ ] What is the confidence in the evidence, and what information is missing?

## Illustrative severity scale

Adapt labels and thresholds to the local incident process.

| Severity | Example impact | Initial coordination |
| --- | --- | --- |
| Critical | A critical service is unavailable broadly, or there is credible safety, security, or significant data-integrity impact. | Immediate incident coordination and specialist/security escalation as applicable. |
| High | A major service or important function is materially degraded for many users; workaround is limited or risky. | Expedite investigation, engage service owner, and provide regular updates. |
| Moderate | A limited group or non-critical function is affected, with a reasonable workaround. | Work through the active queue with a clear owner and follow-up. |
| Low | Minor inconvenience or isolated issue with little business impact and a safe workaround. | Schedule or handle according to normal queue capacity. |

## Setting and reviewing priority

1. Assign an initial severity from verified impact, not the requester’s preferred label.
2. Select priority using severity plus urgency, dependencies, and time constraints under the applicable local matrix.
3. Record the reason, assumptions, workaround, and next review time. Avoid implying a response-time commitment unless one is defined by the service process.
4. Reassess when scope changes, new evidence appears, or the workaround fails. Preserve the history of rating changes.
5. Communicate the current impact and next update point in plain language.

## Example

In a fictional distribution office, one employee cannot open a reporting dashboard but can use a safe exported report. This may be moderate severity and normal priority. If the same failure expands across sites near a time-sensitive reporting deadline, impact and urgency increase; reassess the incident and coordinate with the service owner.

## Escalate promptly when

- There may be a security incident, safety impact, data loss/corruption, or a broad outage.
- Scope is growing, a critical dependency is affected, or the current owner cannot restore service.
- Classification is uncertain and delay could increase harm. Ask the incident lead or service owner to help assess rather than delaying action to perfect a label.

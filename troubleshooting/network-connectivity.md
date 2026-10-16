# Network Connectivity Troubleshooting

Use this guide when a user or device cannot reach a network resource. Start by identifying what is affected; avoid assuming that every connectivity symptom is a network-wide outage.

## Symptoms

- A device reports no internet or cannot reach an internal service.
- One application or hostname fails while other destinations work.
- Wi-Fi disconnects repeatedly, or a VPN connects without providing access to expected resources.
- Users in one location or network segment report similar failures.

## Investigation

1. **Establish scope.** Record the affected user, device, location, network (wired, Wi-Fi, or VPN), destination, start time, and exact error. Ask whether colleagues or other services are affected.
2. **Check local state.** Confirm airplane mode is off, the correct network is selected, and the device has a valid network address, gateway, and DNS configuration. Use approved operating-system diagnostics such as `ipconfig /all` on Windows or `ip addr` and `ip route` on Linux.
3. **Test in layers.** Check link/Wi-Fi association, then the default gateway, then a known internal destination and an approved external destination. Use `ping` only where ICMP is permitted; a failed ping alone does not prove a service is unavailable.
4. **Separate name resolution from reachability.** Resolve the affected hostname with the configured resolver (for example, `nslookup` or `dig`) and compare with a known-good hostname. Do not substitute public DNS or edit host files without authorization.
5. **Check the path and service.** If allowed, use `tracert`/`traceroute` to locate where a path stops. Confirm whether the destination service is healthy and whether a proxy, firewall, VPN route, or recent approved network change could affect it.
6. **Compare.** Test the same destination from a known-good device or network, taking care not to expose credentials or sensitive data.

## Possible causes

- Weak wireless signal, access point issue, disabled adapter, or damaged cable.
- Incorrect or expired DHCP lease, gateway, subnet, or DNS settings.
- DNS record or resolver issue.
- VPN tunnel, route, proxy, firewall rule, or captive portal behavior.
- Destination service outage or a network change affecting a segment.

## Resolution and verification

- Correct simple local issues within the support role, such as reconnecting to the approved SSID or reseating a cable. Renew a lease or restart a network adapter only when appropriate and authorized.
- Do not disable security controls, change firewall rules, or bypass VPN/proxy requirements as a diagnostic shortcut.
- Verify the original destination and workflow, not just general internet access. Confirm stability over a reasonable interval and with the requester when available. Record tests and results.

## Escalate when

- Multiple users, a location, or a critical business service are affected.
- Evidence points to core network, DNS, firewall, VPN, or provider infrastructure outside the support role.
- There is a suspected security event, unexplained route/DNS change, or service degradation with significant business impact.
- Basic checks do not isolate the cause or a change would require elevated access or formal approval.

Include affected scope, timestamps, locations, network type, destination, address/DNS results (redacted as needed), tests performed, and recent relevant changes in the handoff.

# SOC Monitoring Lab

## Objective
Simulate a Security Operations Center (SOC) environment to detect and investigate suspicious login attempts and system events.

---

## Environment
- Windows Server 2019
- SIEM Platform (Wazuh / ELK)
- Windows 10 Client Machine

---

## Implementation Steps

1. Installed and configured SIEM server.
2. Integrated Windows Security Logs.
3. Enabled audit policies (logon events, account lockout).
4. Generated brute-force login simulation.
5. Created custom alert rules for failed login attempts.

---

## Detection Logic

- Event ID 4625 → Failed login attempt
- Multiple failed attempts from same IP
- Account lockout events
- Suspicious login outside business hours

---

## Investigation Process

- Identified source IP
- Reviewed authentication logs
- Correlated failed attempts
- Verified account status
- Assessed risk level

---

## Remediation

- Blocked suspicious IP
- Reset affected account password
- Enabled stricter lockout policy
- Documented incident

---

## Skills Demonstrated

- Log Analysis
- Alert Investigation
- Basic Threat Detection
- Incident Documentation

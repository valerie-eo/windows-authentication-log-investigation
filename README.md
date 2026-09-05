# windows-authentication-log-investigation
# Windows Authentication Log Investigation

## SOC Project 01

A hands-on SOC investigation of Windows authentication events using **Windows Event Viewer** and the **Windows Security Log**.

### Objective

The purpose of this project was to analyse Windows authentication activity, understand different logon types, and determine whether observed events were consistent with normal system behaviour or required further investigation.

### Events Investigated

* **Event ID 4624** — Successful Logon

  * `UMFD-0` — Logon Type 2 (Interactive)
  * `SYSTEM` — Logon Type 5 (Service)

* **Event ID 4625** — Failed Logon

  * Logon Type 2 (Interactive)
  * Source: `127.0.0.1`
  * Process: `svchost.exe`

### Key Findings

The reviewed events appeared predominantly consistent with normal Windows system and service activity. No clear indicators of remote brute-force activity, unauthorized remote access, or successful compromise were identified within the events investigated.

The investigation also demonstrated the importance of analysing authentication events in context rather than relying solely on Event IDs or logon types.

### Tools

* Windows Event Viewer
* Windows Security Logs
* Windows Virtual Machine

### Skills Demonstrated

**Windows Log Analysis · Authentication Analysis · Event ID Analysis · Logon Type Analysis · SOC Investigation · Evidence-Based Assessment**

### Project Files

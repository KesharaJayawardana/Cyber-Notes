# SOC Operations — Overview

## What is a SOC?
A Security Operations Center (SOC) is a team and set of tools that monitor, detect, and respond to cybersecurity incidents across an organisation.

## Common SOC roles
- **Tier 1 (Alert Triage):** Monitor dashboards, validate alerts, do initial enrichment.  
- **Tier 2 (Investigation):** Deep-dive on suspicious events, collect forensic data, recommend containment.  
- **Tier 3 (Threat Hunting / Forensics):** Proactive hunts, malware analysis, root-cause.  
- **SOC Manager:** Coordinates team, reporting, playbooks and escalation.

## Core tools & concepts (high-level)
- **SIEM:** Collects logs, correlates events, creates alerts.  
- **EDR:** Endpoint Detection & Response — visibility into endpoints.  
- **Network monitoring:** IDS/IPS and flow data for network anomalies.  
- **Ticketing / case management:** Track incidents from open → resolved.

## Simple triage process (safe, high-level)
1. **Acknowledge** the alert and record basic info (time, source).  
2. **Enrich** with context (user, asset owner, machine name, recent changes).  
3. **Investigate** logs and telemetry to determine scope (do not perform destructive actions).  
4. **Escalate** to higher tier or incident response if needed.  
5. **Contain & Remediate** following company playbooks.  
6. **Close & Document** lessons learned and update playbooks.

## Quick notes for learning
- Practice reading logs (Windows Event, syslog) and understanding timestamps.  
- Learn common alerts: suspicious login, unexpected process execution, data exfil patterns.  
- Always work in authorized lab environments when practicing.

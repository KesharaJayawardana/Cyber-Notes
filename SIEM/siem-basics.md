# SIEM — Basics (Starter)

## What is a SIEM?
A SIEM (Security Information and Event Management) centralises log collection, normalises data, correlates events, and generates alerts to help detect security incidents.

## Core functions
- **Log collection:** Gather logs from endpoints, servers, network devices, and cloud services.  
- **Normalization & parsing:** Convert different log formats into a common structure.  
- **Correlation:** Combine multiple events to identify suspicious patterns.  
- **Alerting:** Generate actionable alerts for analysts.  
- **Dashboards & reporting:** Visualise trends and produce compliance reports.

## Common SIEM tasks to learn
- Configure log sources (Windows Event, syslog, cloud logs).  
- Write / tune correlation rules to reduce false positives.  
- Search logs with queries (time ranges, host, user, event ID).  
- Build dashboards for common use cases (login failures, malware alerts).  
- Create incident playbooks for common alerts.

## Example simple use-cases
- Repeated failed logins → potential brute-force.  
- New admin account creation → investigate legitimacy.  
- Large data transfer from workstation → possible exfiltration.

## Tips for practice
- Start with a free/trial SIEM (Splunk trial, Elastic + Beats).  
- Forward a few log types (Windows, Linux syslog) and practise queries.  
- Keep rule sets small and test them to avoid noise.

## Ethics & safety
- Only collect and test logs from systems you own or have permission to monitor.

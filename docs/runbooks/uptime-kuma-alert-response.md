# Uptime Kuma Alert Response Runbooks

## Purpose

This page is the index for Uptime Kuma alert response runbooks.

Each child page documents how to respond to a specific alert, what the alert means, what systems may be affected, what checks should be performed first, and how to validate recovery.

## How to Use These Runbooks

1. Open the matching runbook when a Discord alert fires.
2. Confirm the alert status in Uptime Kuma.
3. Perform first checks before restarting services.
4. Follow the recovery steps only after confirming the issue.
5. Validate that the monitor returns to Up.
6. Confirm Discord receives a recovery notification.
7. Record the suspected cause if one is identified.

## Alert Destination

Uptime Kuma notifications are sent to the private Discord alert channel.

Notification name:

HomeLab Critical Alerts

## Runbook Index

| Alert | Runbook |
|---|---|
| Netdata Web DOWN | Runbook - Netdata Web Down |
| Pi-hole DNS DOWN | Runbook - Pi-hole DNS Down |
| Gateway Router DOWN | Runbook - Gateway Router Down |
| Wazuh Dashboard DOWN | Runbook - Wazuh Dashboard Down |
| Samba TCP 445 DOWN | Runbook - Samba TCP 445 Down |
| Omada Controller DOWN | Runbook - Omada Controller Down |
| Internet Checks DOWN | Runbook - Internet Checks Down |
| pi-netutil-01 DOWN | Runbook - pi-netutil-01 Down |
| ER605 / EAP610 / TL-SG108PE DOWN | Runbook - Network Device Down |

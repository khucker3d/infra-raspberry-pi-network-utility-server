# 2. Secure SSH Administration

## Overview

This document describes the sanitized SSH administration model used for managing the Raspberry Pi network utility server.

SSH provides secure command-line access for system updates, service management, log review, backup tasks, and troubleshooting.

## Purpose

The goal of the SSH administration setup is to support secure internal management while avoiding unnecessary exposure of administrative services.

## Access Model

SSH access is designed around the following principles:

* Internal network access only
* Administration from trusted devices
* No public WAN exposure
* No port forwarding from the internet
* Strong authentication practices
* Minimal administrative access

## High-Level Access Flow

```
Trusted Admin Workstation
        |
        | SSH
        |
Internal Network
        |
        | Restricted Administrative Access
        |
Raspberry Pi Utility Server
```

## Administration Use Cases

SSH is used for:

* Operating system updates
* Service installation
* Service restart and validation
* Log review
* Storage mount verification
* Backup execution
* Troubleshooting
* Configuration review

## Security Considerations

The public version of this project does not include:

* SSH usernames
* Internal IP addresses
* Private keys
* Public keys
* Host fingerprints
* Exact firewall rules
* Administrative command history
* File system paths containing sensitive names

## Recommended Hardening Practices

The following practices are appropriate for this type of setup:

* Use SSH only on the internal network
* Disable unused services
* Keep the operating system updated
* Use strong authentication
* Avoid password reuse
* Restrict administrative accounts
* Review logs periodically
* Back up configuration before major changes
* Document recovery procedures

## Operational Notes

SSH access should be treated as an administrative control plane. Any changes made through SSH should be documented when they affect infrastructure behavior, security posture, monitoring, or recovery procedures.

## Skills Demonstrated

This setup demonstrates:

* Linux remote administration
* Secure access planning
* Administrative workflow design
* Service validation
* Infrastructure troubleshooting
* Security-conscious documentation

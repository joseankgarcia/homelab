# Homelab Hardening Checklist

> A concise checklist of core security controls used to harden the homelab environment.

---

## Security Baseline

| Control | Status | Notes |
|---|---|---|
| No Public Ingress | ✅ | Services are not directly exposed to the public internet |
| Overlay Remote Access | ✅ | Remote access is handled through NetBird |
| VLAN Segmentation | ✅ | Client, management, and services traffic are separated |
| Management Isolation | ✅ | Router, switch, and admin interfaces are restricted to management access |
| Firewall Rule Review | ✅ | Traffic is controlled between network zones |
| DNS Filtering | ✅ | Pi-hole is used for DNS filtering |
| Reverse Proxy Control | ✅ | Internal services are routed through a controlled proxy layer |
| SSH Key Authentication | ✅ | Administrative access uses key-based authentication |
| Container Stack Separation | ✅ | Services are organized into separate Docker stacks |
| Centralized Monitoring | ✅ | Grafana, Prometheus, Loki, and Alertmanager provide visibility |
| Log Collection | ✅ | Promtail collects service and container logs |
| Configuration Versioning | ✅ | Compose files and documentation are tracked in Git |
| Backup Planning | 🟡 | Backup strategy is being documented and expanded |
| MFA for Admin Tools | 🟡 | MFA will be added where supported |
| Vulnerability Review | 🟡 | Periodic review process planned for services and containers |

---

---

## Legend

| Symbol | Meaning |
|---|---| 
| ✅ | Implemented |
| 🟡 |  In Progress |

---



## Summary

This homelab follows a private-by-default security model. Services are segmented by network role, administrative access is restricted, and remote connectivity is handled through an encrypted overlay network instead of direct public exposure.

The goal of this checklist is to document practical security controls that improve resilience, reduce attack surface, and demonstrate secure infrastructure design.

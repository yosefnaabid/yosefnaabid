# Yosef Naabid Gutiérrez

**Linux Systems Administrator** · infrastructure as code · virtualization · network security

> I break what I run before I trust it.

Sole sysadmin for a 24/7 hosting production. Everything I manage lives in Git,
gets monitored, and has to prove it can be restored.

## What I run

- **20+ containerized services** on one host, each with CPU/memory limits and
  auto-restart, so a runaway service can't drag down the rest (Docker, Nginx).
- **Admin plane off the internet**: access only through a WireGuard tunnel
  terminated at the router, intrusion attempts blocked automatically
  (MikroTik RouterOS, CrowdSec, nftables).
- **10-minute RTO** for the production database, verified by a monthly restore
  drill in an isolated environment (PostgreSQL).
- **Failures detected in under a minute**, services recover without human
  intervention (Prometheus, Alertmanager, systemd).
- **Full stack rebuildable from scratch in ~15 minutes** — which is how it
  moved to a new dedicated server without clients noticing (Ansible, Bash, Git).

Before that: systems and networks for a university dental-clinic group
(90 sites across 27 countries) — 20 physical servers migrated to VMware and
Proxmox HA clusters, GDPR-audited immutable backups, and Zabbix/Grafana
monitoring for 10 clinics and 300 users.

## Proof, not claims

- **[network-segmentation-lab](https://github.com/yosefnaabid/network-segmentation-lab)** —
  Firewall policy as code: a 6-VLAN network on Proxmox + OPNsense where the
  rules are compiled from a single YAML policy, and a pytest suite in CI proves
  inter-VLAN isolation still holds after every change. Terraform, Ansible,
  chaos testing.
- **[activedirectory-lab](https://github.com/yosefnaabid/activedirectory-lab)** —
  Windows Server domain built and CIS-hardened entirely from PowerShell — DHCP,
  GPOs, CSV-driven user lifecycle — plus a RHEL node joined to the domain
  behind a Squid proxy. Pester tests and PSScriptAnalyzer in CI.
- **[proxmox-backup-lab](https://github.com/yosefnaabid/proxmox-backup-lab)** —
  Backup and disaster recovery on Proxmox VE, automated end to end with Ansible
  and verified with real restores — an untested backup is a hope, not a backup.
- **[zabbix-lab](https://github.com/yosefnaabid/zabbix-lab)** —
  Zabbix 6 monitoring on Debian 12, provisioned by code: server, agent, hosts,
  triggers and alerting registered through the API.
- **[yosefnaabid.com](https://yosefnaabid.com)** — my site and CV, self-hosted
  on Azure.

## Stack

| Area | Tools |
|---|---|
| Systems & virtualization | Linux (Debian, RHEL, AlmaLinux), Windows Server, Proxmox VE, VMware ESXi/vCenter, Hyper-V |
| Network & security | OPNsense, nftables, WireGuard, MikroTik RouterOS, Sophos XGS, CrowdSec, SELinux, Nginx, Cloudflare, VLAN/DHCP/DNS |
| Automation & IaC | Ansible, Terraform, Bash, PowerShell, Python (pytest), Docker, Git, GitHub Actions |
| Monitoring, backup & data | Prometheus, Alertmanager, Grafana, Zabbix, Veeam, PostgreSQL |
| Identity | Active Directory (GPO, LDAP), Entra ID |

**Certifications:** CCNA 200-301 · Azure AZ-104 · ITIL Foundation · Google Cybersecurity · CompTIA Security+ (in progress)

**Languages:** Spanish (native) · English (B2, Cambridge)

## Contact

Open to Linux systems administration roles — anywhere in Spain (on-site or
remote) and remote international.

📫 **yosefnaabid@gmail.com** · [LinkedIn](https://www.linkedin.com/in/yosefnaabid) · [yosefnaabid.com](https://yosefnaabid.com)

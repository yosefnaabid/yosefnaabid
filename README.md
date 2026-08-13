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

**Systems & virtualization**

![Debian](https://img.shields.io/badge/Debian-A81D33?logo=debian&logoColor=white)
![RHEL](https://img.shields.io/badge/RHEL-EE0000?logo=redhat&logoColor=white)
![AlmaLinux](https://img.shields.io/badge/AlmaLinux-0F4266?logo=almalinux&logoColor=white)
![Windows Server](https://img.shields.io/badge/Windows_Server-0078D4)
![Proxmox VE](https://img.shields.io/badge/Proxmox_VE-E57000?logo=proxmox&logoColor=white)
![VMware](https://img.shields.io/badge/VMware_ESXi%2FvCenter-607078)

**Network & security**

![OPNsense](https://img.shields.io/badge/OPNsense-D94F00?logo=opnsense&logoColor=white)
![WireGuard](https://img.shields.io/badge/WireGuard-88171A?logo=wireguard&logoColor=white)
![nftables](https://img.shields.io/badge/nftables-1A1A1A)
![MikroTik](https://img.shields.io/badge/MikroTik_RouterOS-293239)
![CrowdSec](https://img.shields.io/badge/CrowdSec-121C3A)
![Nginx](https://img.shields.io/badge/Nginx-009639?logo=nginx&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?logo=cloudflare&logoColor=white)

**Automation & IaC**

![Ansible](https://img.shields.io/badge/Ansible-EE0000?logo=ansible&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-844FBA?logo=terraform&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?logo=gnubash&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?logo=githubactions&logoColor=white)

**Monitoring, backup & data**

![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?logo=grafana&logoColor=white)
![Zabbix](https://img.shields.io/badge/Zabbix-D40000)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![Veeam](https://img.shields.io/badge/Veeam-00B336)

**Also:** Hyper-V · Sophos XGS · SELinux · Alertmanager · Active Directory (GPO, LDAP) · Entra ID · VLAN / DHCP / DNS · Git · pytest / Pester

**Certifications:** CCNA 200-301 · Azure AZ-104 · ITIL Foundation · Google Cybersecurity · CompTIA Security+ (in progress)

**Languages:** Spanish (native) · English (B2, Cambridge)

## Contact

Open to Linux systems administration roles — anywhere in Spain (on-site or
remote) and remote international.

📫 **yosefnaabid@gmail.com** · [LinkedIn](https://www.linkedin.com/in/yosefnaabid) · [yosefnaabid.com](https://yosefnaabid.com)

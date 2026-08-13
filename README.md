# Yosef Naabid Gutiérrez

**Systems Administrator, Linux and Windows** · infrastructure as code · virtualization · network security

> I break what I run before I trust it.

I am the only sysadmin behind a hosting production that runs 24/7. Everything I manage lives in Git and gets monitored. If I have never restored it, I assume the backup does not exist.

## What I run

* More than 20 containerized services on one host, each with its own CPU and memory limits and automatic restarts, so one runaway service cannot drag down the rest (Docker, Nginx).
* Administration happens off the internet. The only way in is a WireGuard tunnel that ends at the router, and intrusion attempts get blocked without anyone touching a thing (MikroTik RouterOS, CrowdSec, nftables).
* The production database has a recovery time of 10 minutes. I know because I restore it every month in an isolated environment, following a written procedure (PostgreSQL).
* Failures raise an alert in under a minute and services recover on their own (Prometheus, Alertmanager, systemd).
* The whole stack rebuilds from scratch in about 15 minutes with Ansible, Bash and Git. That is how it moved to a new dedicated server without a single client noticing.

Before this I ran systems and networks for a university dental clinic group with 90 sites in 27 countries. I migrated 20 physical servers to 25 virtual machines across VMware and Proxmox clusters in high availability. The clinical data backups were immutable and restore tested, and they passed a GDPR audit. Monitoring ran on Zabbix and Grafana for 10 clinics and around 300 users. I also cut more than 5,000 euros a year in Microsoft 365 licensing after auditing with PowerShell what each seat really used.

## Projects

* **[network-segmentation-lab](https://github.com/yosefnaabid/network-segmentation-lab)** is a network of six VLANs on Proxmox and OPNsense where the firewall rules are compiled from one YAML policy file. A pytest suite runs in CI and proves that traffic between VLANs stays blocked after every change. Terraform and Ansible handle provisioning, with some chaos testing on top.
* **[activedirectory-lab](https://github.com/yosefnaabid/activedirectory-lab)** is a Windows Server domain built from PowerShell alone and hardened with the CIS Benchmark. It covers DHCP, GPOs, user lifecycle fed from CSV files, and a RHEL node joined to the domain behind a Squid proxy. Pester tests and PSScriptAnalyzer run in CI.
* **[proxmox-backup-lab](https://github.com/yosefnaabid/proxmox-backup-lab)** automates backup and disaster recovery on Proxmox VE with Ansible, end to end, and verifies it with real restores.
* **[zabbix-lab](https://github.com/yosefnaabid/zabbix-lab)** builds Zabbix 6 monitoring on Debian 12 from code. Server, agent, hosts, triggers and alerting all get registered through the API.
* **[yosefnaabid.com](https://yosefnaabid.com)** is my site and CV. I host it myself on Azure.

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

On top of those I also work with Hyper-V, Sophos XGS, SELinux, Alertmanager, Active Directory (GPO, LDAP), Entra ID, VLANs, DHCP, DNS, Git, pytest and Pester.

I hold the CCNA 200-301, Azure AZ-104, ITIL Foundation and Google Cybersecurity certifications, and I am preparing CompTIA Security+.

Spanish is my first language. I work in English as well (B2, Cambridge certified).

## Contact

Open to systems administration roles anywhere in Spain, on site or remote, and to international remote work. I work across Linux, Windows and hybrid environments.

Write to **yosefnaabid@gmail.com**, find me on [LinkedIn](https://www.linkedin.com/in/yosefnaabid), or read the CV at [yosefnaabid.com](https://yosefnaabid.com).

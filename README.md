# Cybersecurity Lab Environment Setup

**A documented, isolated virtual lab for cybersecurity learning and authorized security practice.**

![Cybersecurity](https://img.shields.io/badge/Focus-Cybersecurity-red)
![VirtualBox](https://img.shields.io/badge/Platform-VirtualBox%207.2-blue)
![Kali Linux](https://img.shields.io/badge/Workstation-Kali%20Linux-557C94)
![Lab network](https://img.shields.io/badge/Lab%20network-10.0.0.0%2F24-green)
![Use](https://img.shields.io/badge/Use-Educational-orange)

---

## Project Overview

This project documents the setup of a virtual cybersecurity lab using Oracle VirtualBox and Kali Linux. The lab provides a hands-on environment for learning security fundamentals, including virtual machine and network configuration, while keeping practice isolated and authorized.

> **Safety note:** Keep the lab separate from production, workplace, home, and public networks. Only assess systems that you own or have explicit permission to test.

## Objectives

- Build an isolated virtual lab separate from production and home networks.
- Gain hands-on experience installing and configuring Kali Linux.
- Learn foundational security testing concepts in a controlled environment.
- Practice safely configuring and documenting intentionally vulnerable training machines.
- Keep all testing within systems you own or are explicitly authorized to assess.

## Lab Components

| Component | Configuration |
| --- | --- |
| Virtualization platform | Oracle VirtualBox 7.2 |
| Security workstation | Kali Linux (v2026.1, as shown in the lab notes) |
| Lab network | `10.0.0.0/24` |
| Network boundary | Isolated virtual network; do not use Bridged networking for lab targets |

Use an Internal Network or a properly isolated Host-only Network for lab machines. Check each VM's adapter settings before starting it, and do not connect vulnerable targets to a live network.

## Setup Summary

1. Install VirtualBox and create a virtual machine for Kali Linux.
2. Install Kali Linux using the official installation media and follow its installation guidance.
3. Configure the lab network as an isolated virtual network using the `10.0.0.0/24` range.
4. Attach lab VMs only to the isolated network. Confirm that no adapter is set to **Bridged Adapter**.
5. If adding a target VM, use a deliberately vulnerable training image only within the isolated lab.
6. Take a clean snapshot before experiments and document the configuration and results.

Network details may vary with VirtualBox and guest OS versions; verify the settings in your own environment.

## Lab Screenshots

The following screenshots document the lab setup:

### Kali Linux

![Kali Linux setup](Kali%20linux%20.png)

### Kali Linux settings

![Kali Linux settings](Kali%20linux%20setting%20.png)

### Kali network settings

![Kali network settings](Kali%20network%20setting%20.png)

### Virtual network settings

![Virtual network settings](network%20sett.png)

## Safety Checklist

- [ ] Lab targets are not connected to public, workplace, or home networks.
- [ ] No VM adapter uses Bridged networking for vulnerable targets.
- [ ] Testing is limited to systems owned by you or covered by explicit authorization.
- [ ] Snapshots or backups are available before making changes.
- [ ] Credentials, personal data, and secrets are not stored in the repository.

## Responsible Use

This repository is for education and authorized lab use only. You are responsible for keeping your environment isolated and obtaining permission before assessing any system. Never test public or third-party systems without explicit authorization.

## Author

**Ibrahim Muazzam Abubakar**  
NetworkWalks B084 · Week 1

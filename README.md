# 🔐 Cybersecurity Lab Environment Setup

**Building an isolated virtual lab for cybersecurity learning and ethical security practice.**

![Skill: Cybersecurity](https://img.shields.io/badge/Skill-Cybersecurity-red)
![VirtualBox](https://img.shields.io/badge/VirtualBox-v7.2-blue)
![Kali Linux](https://img.shields.io/badge/Kali%20Linux-v2026.1-557C94)
![Network](https://img.shields.io/badge/Network-10.0.0.0%2F24-green)
![Penetration Testing](https://img.shields.io/badge/Use-Educational-orange)
![Virtualization](https://img.shields.io/badge/Skill-Virtualization-purple)

---

## 📌 Project Overview

This project documents the setup of a virtual cybersecurity lab using VirtualBox and Kali Linux. It is intended as a hands-on, self-guided learning environment for practicing security fundamentals—from virtual machine and network configuration to safe, authorized testing of deliberately vulnerable systems.

The lab should remain isolated from production, home, and other networks. Do not use these materials to access systems without explicit permission.

## 🎯 Objectives

- Build an isolated virtual lab, separate from production and home networks.
- Gain hands-on experience installing and configuring Kali Linux.
- Learn foundational security testing concepts in a controlled environment.
- Understand how to safely configure and document intentionally vulnerable target machines.
- Keep all testing within systems you own or are explicitly authorized to assess.

## 🧰 Lab Components

| Component | Details |
| --- | --- |
| Virtualization platform | Oracle VirtualBox 7.2 |
| Security workstation | Kali Linux (v2026.1, as shown in the lab notes) |
| Lab network | `10.0.0.0/24` |
| Network boundary | Isolated virtual network; do not use Bridged networking for lab targets |

> **Safety first:** Use an Internal Network or a properly isolated Host-only Network for lab machines. Check every VM's adapter settings before starting it, and do not connect vulnerable targets to a live network.

## 🛠️ Setup Summary

1. Install VirtualBox and create a virtual machine for Kali Linux.
2. Install Kali Linux using the official installation media and follow its installation guidance.
3. Configure the lab network as an isolated virtual network using the `10.0.0.0/24` range.
4. Attach lab VMs only to the isolated network. Confirm that no adapter is set to **Bridged Adapter**.
5. If adding a target VM, use a deliberately vulnerable training image in the isolated lab only.
6. Take a clean snapshot before experiments and document the configuration and results.

Specific network details may vary with your VirtualBox and guest OS versions; verify the settings in your own environment.

## 📷 Lab Screenshots

The following screenshots are included in this repository as setup evidence:

### Kali Linux

![Kali Linux setup](Kali%20linux%20%20.png)

### Kali network settings

![Kali network settings](Kali%20network%20setting%20%20.png)

### Virtual network settings

![Virtual network settings](network%20sett.png)

## ✅ Safety Checklist

- [ ] Lab targets are not connected to a public, workplace, or home network.
- [ ] No VM adapter uses Bridged networking for vulnerable targets.
- [ ] Testing is limited to systems owned by you or covered by explicit authorization.
- [ ] Snapshots or backups are available before making changes.
- [ ] Credentials, personal data, and secrets are not stored in the repository.

## ⚖️ Responsible Use

This repository is for education and authorized lab use only. You are responsible for keeping your environment isolated and obtaining permission before assessing any system. Never test against public or third-party systems without explicit authorization.

## 👤 Author

**Ekpenyong Peace** — NetworkWalks B084, Week 1

# 🔐 Zero Trust Identity Lab

> A hands-on, 2-hour lab for Junior Security Analysts demonstrating the transition from Traditional Perimeter Security to Zero Trust Architecture (ZTA), based on **NIST SP 800-207**.

---

## 🌐 Live Lab Guide

👉 **[View the Full Lab Guide](./lab-guide.md)**

---

## 📖 Introduction

Traditional network security assumed that anything inside the network perimeter could be trusted. This "castle and moat" model fails catastrophically when an attacker gets inside — they can move freely across systems.

**Zero Trust flips this assumption:**
> *"Never trust, always verify."*

Every connection, every user, every device must prove its identity — regardless of where it is on the network.

This lab walks you through building a real Zero Trust environment using only free, open-source tools.

---

## 🎯 Learning Objectives

By the end of this lab, you will be able to:

1. **Explain** the difference between perimeter-based and identity-based security
2. **Deploy** Tailscale to create an identity-authenticated mesh network
3. **Write** Tailscale ACL rules to enforce micro-segmentation
4. **Configure** Linux `sudoers` to enforce the Principle of Least Privilege
5. **Use** a Generative AI model as a Security Co-pilot to audit `auth.log` files

---

## 🧰 Prerequisites

### Accounts (all free)
- [ ] GitHub account — [github.com](https://github.com)
- [ ] Tailscale account — [tailscale.com](https://tailscale.com) *(sign up with GitHub)*

### Technical Requirements
- [ ] 2 Linux machines (VMs, cloud instances, or bare metal)
  - Ubuntu 22.04 / Debian / Linux Mint recommended
  - Kali Linux works as a client node
- [ ] Both machines must have internet access
- [ ] Basic comfort with a Linux terminal

### Knowledge
- [ ] Basic Linux command line (cd, ls, sudo)
- [ ] No prior networking or security experience required

---

## 🗺️ Lab Structure

| Milestone | Topic | Est. Time |
|-----------|-------|-----------|
| **0** | Environment Setup | 20 min |
| **1** | Identity-Centric Connectivity | 20 min |
| **2** | Micro-segmentation | 25 min |
| **3** | Principle of Least Privilege | 25 min |
| **4** | GenAI Security Co-pilot | 20 min |
| — | Wrap-up & Review | 10 min |
| **Total** | | **~2 hours** |

---

## 🛠️ Technical Stack

| Layer | Tool | Purpose |
|-------|------|---------|
| Network | [Tailscale](https://tailscale.com) | ZTNA & identity-based mesh networking |
| Compute | Linux (Ubuntu/Mint/Kali) | Lab environment |
| Identity | GitHub SSO via Tailscale | OIDC-based authentication |
| Access Control | Tailscale ACLs (JSON) | Network-layer micro-segmentation |
| Access Control | Linux `sudoers` | Host-layer RBAC / Least Privilege |
| Monitoring | `auth.log` + GenAI | Security auditing & co-pilot analysis |

---

## 📚 References

- [NIST SP 800-207 — Zero Trust Architecture](https://csrc.nist.gov/publications/detail/sp/800-207/final)
- [Tailscale ACL Documentation](https://tailscale.com/kb/1018/acls)
- [Linux sudoers Manual](https://www.sudo.ws/docs/man/sudoers.man/)

---

## 👤 Author

Built as part of a Zero Trust & Identity internship technical challenge.  
Stack: Tailscale · Linux Mint · Kali Linux · GitHub SSO · ufw · sudoers

---
layout: post
title: Active Directory Reconnaisance
categories: [Automation,Recon,]
author: alucab
---

## Overview

## Tools
### [ADRecon](https://github.com/sense-of-security/ADRecon)

ADRecon is a tool which extracts various artifacts (as highlighted below) out of an AD environment in a specially formatted Microsoft Excel report that includes summary views with metrics to facilitate analysis. The report can provide a holistic picture of the current state of the target AD environment. The tool is useful to various classes of security professionals like system administrators, security professionals, DFIR, etc. It can also be an invaluable post-exploitation tool for a penetration tester. It can be run from any workstation that is connected to the environment, even hosts that are not domain members. Furthermore, the tool can be executed in the context of a non-privileged (i.e. standard domain user) accounts. Fine Grained Password Policy, LAPS and BitLocker may require Privileged user accounts. The tool will use Microsoft Remote Server Administration Tools (RSAT) if available, otherwise it will communicate with the Domain Controller using LDAP.

The following information is gathered by the tool: Forest; Domain; Trusts; Sites; Subnets; Default Password Policy; Fine Grained Password Policy (if implemented); Domain Controllers, SMB versions, whether SMB Signing is supported and FSMO roles; Users and their attributes; Service Principal Names (SPNs); Groups and memberships; Organizational Units (OUs); ACLs for the Domain, OUs, Root Containers and GroupPolicy objects; Group Policy Object details; DNS Zones and Records; Printers; Computers and their attributes; LAPS passwords (if implemented); BitLocker Recovery Keys (if implemented); and GPOReport (requires RSAT).

### Other tools
https://github.com/aikoncwd/vbs-ad-health-report
https://github.com/lefayjey/linWinPwn
https://github.com/S3cur3Th1sSh1t/WinPwn

## Cheat Sheets & Workflows

https://github.com/S1ckB0y1337/Active-Directory-Exploitation-Cheat-Sheet
https://github.com/Integration-IT/Active-Directory-Exploitation-Cheat-Sheet

## Commercial Projects
###[PingCastle](https://www.pingcastle.com)
De Facto standard for AD Security Hardening

## Articles 
[Linux Machines in Active Directory](https://blog.workinghardinit.work/2021/05/04/linux-ad-computer-object-operating-system-values/)
[Query AD from Centos](https://stackoverflow.com/questions/26212854/how-to-get-a-list-with-all-the-hosts-connected-to-a-domain-centos-6-5)
[using Get-ADcomputer on PCs without AD rsat installed](https://www.reddit.com/r/PowerShell/comments/10dhvie/using_getadcomputer_on_pcs_without_ad_rsat/)
[Attacking AD](https://medium.com/@rajeevranjancom/attacking-active-directory-3109534290e8)
[Retrieve Computers Info w. Powershell](https://sid-500.com/2019/07/30/powershell-retrieve-list-of-domain-computers-by-operating-system/)
[How to get OU details of a VM Hyper-V](https://community.broadcom.com/vmware-cloud-foundation/discussion/how-to-get-ou-details-of-a-vm)
[Get all VMs with Running OS Like Linux or Other](https://community.broadcom.com/vmware-cloud-foundation/discussion/get-all-vms-with-running-os-like-linux-or-other-script)
[Get a List of Virtual Machines by Using PowerShell](https://devblogs.microsoft.com/scripting/get-a-list-of-virtual-machines-by-using-powershell/)
[Get IP address of your VMs](https://superuser.com/questions/961847/get-ip-addresses-of-hyper-v-linux-machines)


# Perform System Configuration Gap Analysis

## Overview
In this lab, I performed a system configuration gap analysis on a Windows Server 2019 system. I compared the system's current security configuration against a recommended security baseline to identify configuration differences.

## Environment
- Windows Server 2019
- Microsoft Policy Analyzer
- Windows PowerShell
- Microsoft Security Baseline

## Tasks Performed
- Prepared the Windows Server lab environment using PowerShell.
- Extracted and launched Microsoft Policy Analyzer.
- Loaded a Windows Server 2019 security baseline.
- Compared the system configuration against the security baseline.
- Reviewed policy settings that differed from the recommended baseline.
- Identified configuration gaps that could affect system security.

## Example Finding
Reviewed the `LockBadCount` policy setting, which controls the number of failed login attempts allowed before an account is locked.

The security baseline recommended:

**Account lockout threshold: 10 invalid logon attempts**

This demonstrated how security baselines can be used to identify differences between an organization's current configuration and its recommended security configuration.

## Lab Evidence

<img width="1325" height="753" alt="image" src="https://github.com/user-attachments/assets/dc6aeb52-5811-444f-9689-2ece62fc2ab7" />

The following Policy Analyzer result shows the Windows Server security baseline setting for the account lockout threshold (`LockoutBadCount`). The recommended baseline value is **10 failed logon attempts**.

## Skills Practiced
- Security configuration analysis
- Gap analysis
- Security baselines
- Windows Server security
- Microsoft Policy Analyzer
- Windows PowerShell
- Security policy review

## What I Learned
I learned that a gap analysis does not automatically fix security problems. It identifies differences between the current system configuration and the expected security baseline. These findings can then be reviewed to determine whether configuration changes are necessary.

I also learned that security baselines should match the appropriate operating system, product version, and build because one security template may not be appropriate for every system.

# Home SOC & DFIR Lab Architecture

## 1. Purpose

This document describes the environment used for hands-on Security Operations Center (SOC) and Digital Forensics and Incident Response (DFIR) learning.

## 2. Host Environment

- **Host operating system:** Windows 11
- **Virtualization platform:** VMware Workstation
- **Memory:** 16 GB RAM
- **Processor:** Intel Core i5-13420H
- **Existing virtual machine:** Kali Linux

## 3. Current Investigation Workflow

1. Windows generates system and security events.
2. Windows Event Viewer is used to review available event records.
3. PowerShell is used for file-signature verification and cryptographic hashing.
4. Observations are documented in case notes and a structured investigation timeline.
5. Findings are assessed with explicit limitations and without assuming that an alert or event proves malicious activity.

## 4. Planned Architecture

The next phase will assess a suitable SIEM deployment, potentially Wazuh, based on available host resources.

Planned activities include:

- Evaluating a resource-appropriate SIEM setup.
- Configuring endpoint telemetry collection.
- Generating controlled, authorized test activity.
- Reviewing alerts and validating detection results.
- Documenting investigation findings and limitations.

## 5. Network and Safety Considerations

Virtual machines will be configured deliberately for the intended lab activity. Network mode alone does not guarantee isolation. Simulations will be limited to systems and networks for which testing is authorized.

## 6. Current Status

**Status:** Windows endpoint log review and initial file verification completed. SIEM deployment and detection validation are pending.

This architecture document will be updated as the lab evolves.

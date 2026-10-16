# Home SOC & DFIR Investigation Lab

A hands-on cybersecurity lab focused on Windows endpoint investigation, security event analysis, file verification, and Security Operations Center (SOC) workflows.

## Project Overview

This project documents the development of a home-based SOC and Digital Forensics & Incident Response (DFIR) lab. It focuses on collecting and interpreting endpoint telemetry, investigating Windows security events, validating file attributes, and documenting evidence-based findings.

The lab is being developed incrementally, with an emphasis on repeatable procedures, accurate interpretation, and clear investigation reports.

## Objectives

- Investigate Windows Security events and identify relevant fields.
- Understand Windows logon events and process-creation telemetry.
- Practise file signature verification and SHA-256 hashing.
- Develop structured investigation timelines and case documentation.
- Integrate a Security Information and Event Management (SIEM) platform.
- Build and validate detection and investigation workflows in a controlled environment.

## Lab Environment

- **Host OS:** Windows 11
- **Virtualization:** VMware Workstation
- **Virtual machine:** Kali Linux
- **Endpoint investigation tools:** Windows Event Viewer and PowerShell
- **Planned SIEM:** Wazuh

## Work Completed

- Reviewed Windows Security Event ID 4624 (successful logon).
- Checked for Event ID 4625 (failed logon) and documented the limits of the available search results.
- Examined Event ID 4688 (process creation) and recorded process-related fields.
- Checked the Authenticode signature status of a Windows executable using PowerShell.
- Calculated a SHA-256 hash using PowerShell.
- Began documenting findings in a structured investigation timeline.

## Planned Work

- Finalize the initial Windows event investigation case study.
- Document lab architecture and telemetry flow.
- Deploy and configure Wazuh when the host resource plan is ready.
- Collect endpoint telemetry and investigate generated alerts.
- Conduct controlled detection tests and document results.
- Publish sanitized screenshots and a final investigation report.

## Investigation Approach

Findings are documented by distinguishing observed evidence, interpretation, limitations, and follow-up actions. An event or indicator is not treated as proof of malicious activity without sufficient corroborating evidence.

## Repository Structure

The repository structure will expand as the lab develops.

- `docs/` — Lab architecture, setup, and methodology
- `cases/` — Investigation notes, timelines, and reports
- `detections/` — Detection logic and validation results
- `scripts/` — Supporting PowerShell and Python scripts
- `screenshots/` — Sanitized screenshots documenting completed work

## Disclaimer

This project is for educational and defensive cybersecurity purposes. Testing will be conducted only in controlled environments and on systems for which authorization is available.

**Project status:** In progress

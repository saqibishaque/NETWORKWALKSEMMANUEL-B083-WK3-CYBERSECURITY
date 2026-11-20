# NetworkWalks Academy — Week 3 Security Assessment

Password-cracking security assessment completed for the Week 3 internship project modules at [NetworkWalks Academy](https://networkwalks.com).

## Overview

This repository documents the completion of both Week 3 essential project modules:

- **PM1** — Password Cracking with John the Ripper (JTR)
- **PM2** — Password Cracking with NetworkWalks' own Hash Calculator and Password Cracker tools

Four password-protected PDF files were provided for the exercise. All four were cracked using dictionary/wordlist attacks, each confirmed by opening the file and capturing its completion flag.

## Results at a Glance

| File | Password Recovered | Method |
| --- | --- | --- |
| `My Locked PDF1.pdf` | `good-luck` | JTR / Johnny |
| `My Locked PDF2.pdf` | `password1` | JTR / Johnny |
| `My Locked PDF3.pdf` | `1qaz2wsx` | JTR / Johnny |
| `My Locked PDF1 (for NW Tools Lab WK3-PM2).pdf` | `password1` | NetworkWalks Hash Calculator + Password Cracker |

Key observations, written up in full in the formal assessment report:

- All four passwords fell to a wordlist of 100 entries or fewer in under 5 minutes combined
- The password `password1` was reused across two separate files
- All four files used the legacy PDF encryption standard (Revision 4 / AES-128) rather than the current maximum (Revision 6 / AES-256)

## Repository Structure

```text
.
├── README.md
├── reports/
│   └── Internship_Security_Assessment.pdf  # Formal findings report (Executive Summary, Findings, Remediation)
└── evidence/
    ├── screenshots/                         # SS1-SS8 proof-of-concept screenshots
    └── hashes/                              # Extracted $pdf$ hash for each file

Report
📄 Internship Security Assessment — formal findings report with severity ratings, proof of concept, impact, and step-by-step remediation

Tools Used
John the Ripper / Johnny GUI

NetworkWalks Hash Calculator & Password Cracker (networkwalks.com)

Course
NetworkWalks Academy — Cybersecurity & Ethical Hacking, Week 3 Project Modules
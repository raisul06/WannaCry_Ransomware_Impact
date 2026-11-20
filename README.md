# WannaCry Ransomware: Causes, Impact, and Lessons Learned

A comprehensive cybersecurity case study examining the **May 2017 WannaCry ransomware outbreak**, its worm-like propagation via the EternalBlue SMBv1 exploit, operational disruption across the UK National Health Service (NHS), and actionable defense and recovery priorities.

---

## Incident Snapshot

| Attribute | Details |
| :--- | :--- |
| **Incident Date** | 12 May 2017 |
| **Vulnerability** | `CVE-2017-0144` (Windows SMBv1 Remote Code Execution) |
| **Exploit & Patch** | EternalBlue / Microsoft Security Bulletin `MS17-010` |
| **Case Study Focus** | Global Worm Outbreak & NHS in England |
| **Author** | MD Raisul Fahad ([@raisul06](https://github.com/raisul06)) |

---

## Presentation Structure (11 Slides)

1. **Title & Case Overview** — Outbreak summary, incident metadata, and CVE reference (`CVE-2017-0144`).
2. **The Incident** — Overview of WannaCry's self-propagating worm capabilities, global reach, and the ransom demand interface.
3. **Connection to Cybersecurity Concepts** — Analysis through the CIA Triad (**Confidentiality**, **Integrity**, and **Availability**), highlighting how WannaCry disrupted access to essential clinical services.
4. **The Timeline** — Key milestones across the **59-day gap** between Microsoft's `MS17-010` patch release (14 March 2017), the global outbreak (12 May 2017), kill switch activation (12 May 2017), and emergency updates for legacy systems (13 May 2017).
5. **The Vulnerability** — Technical breakdown of Windows **SMBv1** network resource sharing, `CVE-2017-0144`, the **EternalBlue** exploit, and patch `MS17-010`.
6. **How the Attack Spread** — Four-stage automated propagation cycle: **Find** reachable hosts $\rightarrow$ **Exploit** vulnerable SMB services $\rightarrow$ **Propagate** to additional machines $\rightarrow$ **Encrypt** user files.
7. **Impact on the NHS in England** — Operational impact across healthcare providers, including disruption at **81 of 236 trusts ($\ge 34\%$)** and **19,000+ estimated cancelled appointments**.
8. **The Response and the Kill Switch** — Containment via the domain-check kill switch versus recovery of encrypted systems.
9. **Prevention and Recovery Priorities** — Actionable security controls mapped to verification evidence across **Asset Visibility**, **Legacy Protocols (SMBv1 Retirement)**, **Network Access**, **Recovery & Backups**, and **Incident Response Rehearsal**.
10. **Lessons Learned** — Combining verified technical controls (patching and network segmentation) with operational readiness (tested restoration and clear incident roles).
11. **Sources** — Primary government, audit, and vendor technical advisories referenced in the study.

---

## Key Takeaways

- **Timely Patch Management:** Security updates only protect organizations when deployment is verified across all active endpoints (`MS17-010` was released 59 days before the outbreak).
- **Retire Legacy Protocols:** Disabling outdated protocols such as **SMBv1** and restricting lateral network exposure eliminates worm propagation paths.
- **Tested Backups & Continuity:** Because the kill switch halted further spread without decrypting affected systems, offline, restoration-tested backups remain essential for service availability.

---

## Repository Contents

- `WannaCry_Professional_Uniform_Navy-v2.pptx` — 11-slide case study presentation deck
- `README.md` — Project overview, slide breakdown, and primary references

---

## Sources & Primary References

1. **National Audit Office (2017)** — *Investigation: WannaCry cyber attack and the NHS*
2. **Microsoft (14 March 2017)** — *Security Bulletin MS17-010*
3. **Microsoft (May 2017)** — *Customer guidance for WannaCrypt attacks*
4. **Microsoft (12 May 2017)** — *WannaCrypt ransomware worm analysis*
5. **Microsoft (27 June 2017)** — *EternalBlue reference in Petya analysis*
6. **Canadian Centre for Cyber Security** — *Ransomware: WannaCry advisory*

---

## Author

**MD Raisul Fahad**  
GitHub: [@raisul06](https://github.com/raisul06)
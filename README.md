# Digital Forensics Practicals – Autopsy & Guymager

This repository contains lab practical notes and screenshots for two widely used digital forensic tools:
- **Autopsy** – GUI for The Sleuth Kit (TSK) used for disk image analysis and evidence reporting.
- **Guymager** – A forensic disk imaging tool used for creating and verifying forensic images.

---

## 🔍 Guymager

### Overview
Guymager is a Linux-based forensic imaging tool used to acquire bit-by-bit copies of storage devices. It ensures data integrity using hashing and generates detailed acquisition reports.

### Key Features
- Disk imaging and cloning.
- Supports formats: `E01`, `AFF`, `RAW`.
- Integrity verification with MD5/SHA1/SHA256.
- Generates detailed `.info` log files.

### Workflow
1. **Launch Guymager** → Lists all connected drives.
2. **Select Device** → Choose the suspect disk or USB.
3. **Acquire Image** → Enter case details (case number, examiner, evidence number).
4. **Select Format** → RAW, E01, or AFF.
5. **Imaging Process** → Progress bar shows copied data, speed, hash values.
6. **Completion** → A detailed acquisition log is generated for chain-of-custody.

---

## 🕵️ Autopsy

### Overview
Autopsy is a GUI-based forensic platform built on The Sleuth Kit (TSK). It allows investigators to analyze disk images, recover deleted files, build timelines, and generate reports.

### Key Features
- Case management (case name, examiner details).
- Supports multiple evidence sources (disk images, local drives, files).
- File system and metadata analysis (NTFS, FAT, EXT, HFS+).
- Deleted file recovery and keyword search.
- Artifact analysis (web history, emails, registry, chat logs).
- Timeline analysis of system/user activities.
- Export professional forensic reports (HTML, PDF, Excel, CSV).

### Workflow
1. **Start Autopsy** → Launch via CLI (`autopsy`) to open the web interface.
2. **New Case** → Enter case name, case number, examiner.
3. **Add Host** → Define host details (time zone, timeskew, hash databases).
4. **Add Evidence** → Import image (E01/RAW/AFF) using Copy/Symlink.
5. **Hash Verification** → MD5/SHA computed to ensure integrity.
6. **Volume Detection** → Classify partition system (e.g., DOS/MBR).
7. **Evidence Analysis** → Browse files, view metadata, recover deleted data.
8. **Timeline/Artifact View** → Review user activity and system logs.
9. **Report Generation** → Export findings to HTML, PDF, CSV.

---

## 📂 Repository Contents
- `/guymager/` → Screenshots and notes on Guymager workflow.
- `/autopsy/` → Screenshots and notes on Autopsy workflow.
- `README.md` → This documentation.

---

## ⚖️ Disclaimer
These notes and screenshots are for **academic and training purposes only**.  
Do **not** use these tools on unauthorized systems or data.

---

## 👨‍💻 Author
**Clinton Nyamare Orenge**  
Forensics Lab Practicals

# Bruteforce-Project

## 📌 Objective

Learn practical password auditing by running John the Ripper (JtR) on Windows to perform both dictionary and brute‑force attacks against a sample password‑hash file (`hackme.txt`). Capture timestamps and screenshots, and collect cracked passwords in `john.pot` for reporting.


## 🧠 Skills Gained

- Setting up a local security lab folder structure on Windows (`C:\security\`)
- Extracting and running precompiled security tools (JtR Windows binaries)
- Performing dictionary attacks using supplied wordlists (e.g., `password.lst`)
- Running brute‑force attacks and safely interrupting long‑running jobs
- Reading and interpreting the `john.pot` file that stores cracked passwords
- Documenting evidence (timestamps, screenshots) for lab reporting and audit trails
- Understanding the ethical and legal boundaries of password auditing

## 🛠️ Tools & Technologies Used

- John the Ripper (john.exe) — Windows 64‑bit binaries (john‑1.9.0‑jumbo or later)  
- Windows Command Prompt (`cmd.exe`)  
- Supplied sample hash file: `hackme.txt` (course companion files)  
- Built‑in wordlist: `password.lst` (bundled with JtR)  
- Notepad for viewing `john.pot`  
- Screenshot tool (PrtScn / Snipping Tool) for evidence collection

## 🖥️ Lab Environment & File Overview

Component | Details
---|---
Lab Folder | `C:\security\`
JtR Binary Folder | `C:\security\john-1.9.0-jumbo-1-win64\run\`
Sample Hash File | `hackme.txt` (from course companion)
Default Wordlist | `password.lst` (included with JtR)
Output / Pot File | `john.pot` (stores cracked hash → password mappings)
Shell | Windows Command Prompt (`cmd.exe`)

## 🔍 Pre-Lab Setup (Downloads & File Placement)

1. Create folder: `C:\security\`.  
2. Download John the Ripper (Windows 64‑bit binaries) from the official site and extract to `C:\security\john-1.9.0-jumbo-1-win64\`.  
3. Download the course Study Guide and extract `hackme.txt` to `C:\security\`.  
4. Copy `hackme.txt` into `C:\security\john-1.9.0-jumbo-1-win64\run\`.  
5. Confirm `john.exe`, `password.lst`, and `hackme.txt` are in the `run` directory.

## 🧭 Step‑by‑Step Procedure (Commands & Evidence)

> Open Command Prompt (Start → type `cmd` → Enter)

1. Change to the run directory:
   ```bat
   cd \
   cd security
   cd john-1.9.0-jumbo-1-win64
   cd run
   dir

## 🖼️ Screenshots

<img width="750" height="351" alt="Screenshot 2025-10-13 183442" src="https://github.com/user-attachments/assets/5bb2811d-0b6a-4b10-bdd3-29a7646515cc" />

<img width="750" height="288" alt="Screenshot 2025-10-13 183417" src="https://github.com/user-attachments/assets/fcd6c736-b58d-450f-b14f-5168f6f3280a" />

<img width="750" height="640" alt="Screenshot 2025-10-13 181704" src="https://github.com/user-attachments/assets/c40563e5-af28-4757-a8df-0774dfa84396" />

## 📄 Executive Summary

This lab teaches password auditing basics using John the Ripper on Windows. The dictionary attack highlights weak passwords present in common lists while the brute‑force run explores John's incremental cracking power at the cost of time and compute. Documenting runs with timestamps and screenshots produces an audit trail useful for reporting and remediation. The exercise emphasizes ethical constraints: only test authorized sample data and handle any discovered credentials as sensitive information.

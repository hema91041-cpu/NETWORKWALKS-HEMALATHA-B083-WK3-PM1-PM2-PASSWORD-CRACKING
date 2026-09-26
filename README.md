🔓 Password Cracking with JTR & NetworkWalks Tools

**Recovering passwords from protected PDF files using John the Ripper and web-based cracking tools**

`Skill: Cybersecurity` `Tool: John the Ripper` `Tool: Johnny GUI` `OS: Kali Linux` `Skill: Password Auditing` `Skill: Ethical Hacking` `NetworkWalks` `Waqas Karim CCIE`

---

## 📌 Project Overview

This project is part of Week 3 of the NetworkWalks Cybersecurity Internship Program. The objective was to understand how password cracking works by recovering passwords from encrypted PDF files using two different approaches:

1. **W3-PM1** — Password cracking using **John the Ripper (JTR)** and its GUI front-end **Johnny**, run directly on **Kali Linux**.
2. **W3-PM2** — Password cracking using **NetworkWalks' own web-based tools**: the Hash Calculator (to extract the hash) and the Password Cracker (to run a dictionary attack).

Three separate locked PDF files (`My Locked PDF1.pdf`, `My Locked PDF2.pdf`, `My Locked PDF3.pdf`) were cracked as part of this exercise.

---

## 🛠️ Tools & Technologies Used

- **OS:** Kali Linux (JTR pre-installed)
- **Tool 1:** John the Ripper (JTR) — command-line password recovery tool
- **Tool 2:** Johnny — GUI front-end for JTR
- **Tool 3:** NetworkWalks Hash Calculator — https://networkwalks.com/hash-calculator/
- **Tool 4:** NetworkWalks Password Cracker (Dictionary Attack) — https://networkwalks.com/password-cracker/
- **Target Files:** My Locked PDF1.pdf, My Locked PDF2.pdf, My Locked PDF3.pdf

---

## 📋 Steps Performed

### Module 1 — W3-PM1: Password Cracking with JTR (Kali Linux)
1. Opened John the Ripper (pre-installed on Kali Linux) via terminal.
2. Extracted the crackable hash from each locked PDF using `pdf2john`.
3. Saved each extracted hash into its own `.txt` file.
4. Ran John the Ripper (or Johnny GUI) against each hash file to recover the password.
5. Verified the cracked password by opening the corresponding PDF file with it.
6. Repeated the same process for all 3 PDFs (PDF1, PDF2, PDF3).

### Module 2 — W3-PM2: Password Cracking with NetworkWalks Tools
1. Opened the NetworkWalks Hash Calculator in the browser.
2. Uploaded each locked PDF file to extract its `$pdf$...` hash.
3. Copied the complete hash value for each PDF.
4. Opened the NetworkWalks Password Cracker (Dictionary Attack tool).
5. Pasted each hash and ran the attack using the built-in wordlist.
6. Recorded the cracked password once the tool found a match.
7. Opened each PDF using its cracked password to confirm success.

---

## 🖼️ Screenshots & Evidence

### Module 1 — John the Ripper (Kali Linux) — 6 screenshots
*(folder: `PM1/`)*

**PDF 1**
![JTR Hash Extraction PDF1](Module1_JTR/m1-01-pdf1-hash-extract.jpg)
![JTR Cracked Password PDF1](Module1_JTR/m1-02-pdf1-cracked.jpg)

**PDF 2**
![JTR Hash Extraction PDF2](Module1_JTR/m1-03-pdf2-hash-extract.jpg)
![JTR Cracked Password PDF2](Module1_JTR/m1-04-pdf2-cracked.jpg)

**PDF 3**
![JTR Hash Extraction PDF3](Module1_JTR/m1-05-pdf3-hash-extract.jpg)
![JTR Cracked Password PDF3](Module1_JTR/m1-06-pdf3-cracked.jpg)

### Module 2 — NetworkWalks Hash Calculator & Password Cracker — 5 screenshots
*(folder: `PM2/`)*

**PDF 1**
![Hash Calculator PDF1](Module2_NetworkWalksTools/m2-01-pdf1-hashcalc.jpg)
![Password Cracker Result PDF1](Module2_NetworkWalksTools/m2-02-pdf1-cracked.jpg)

**PDF 2**
![Hash Calculator PDF2](Module2_NetworkWalksTools/m2-03-pdf2-hashcalc.jpg)
![Password Cracker Result PDF2](Module2_NetworkWalksTools/m2-04-pdf2-cracked.jpg)

**PDF 3**
![Password Cracker Result PDF3](Module2_NetworkWalksTools/m2-05-pdf3-cracked.jpg)

*(Rename your actual screenshot files to match the names above, in the same order you took them — m1 = Module 1/JTR, m2 = Module 2/NetworkWalks tools. If your order is different, just tell me and I'll update the paths to match.)*

---

## 🔑 Cracked Passwords

| File | Cracked Password (JTR) | Cracked Password (NetworkWalks Tool) |
|---|---|---|
| My Locked PDF1.pdf | *(good-luck)* | *(good-luck)* |
| My Locked PDF2.pdf | *(password1)* | *(passward1)* |
| My Locked PDF3.pdf | *(fill in)* | *(fill in)* |

---

## ⚠️ Troubleshooting Experience

**Problem faced:** *(e.g., "hash extracted from the PDF had extra characters like b' at the start")*

**Solution:** *(e.g., "removed the b' prefix and trailing quote before saving the hash into the .txt file, so John the Ripper could read it correctly")*

*(If no issues were faced, mention helping others with their questions in the video comments instead.)*

---

## 📚 Learnings

- Understood the difference between encryption (two-way, reversible) and hashing (one-way, irreversible).
- Learned how a password-protected PDF stores its password as a hash, and how tools like `pdf2john` extract that hash.
- Learned to use John the Ripper both via command line and via the Johnny GUI on Kali Linux.
- Learned how a dictionary attack works by testing tool-provided wordlists against a hash until a match is found.
- Understood why short, common passwords are cracked quickly, reinforcing the importance of strong passwords.

---

## 🔗 Related Links

- Instructor: [Waqas Karim CCIE](https://linkedin.com/in/waqaskarim/)
- Organization: [NETWORKWALKS](https://linkedin.com/company/networkwalks/)
- Program: NetworkWalks Cybersecurity Internship Program

---

## ⚖️ Disclaimer

This lab was performed strictly for **educational and research purposes** as part of the NetworkWalks Cybersecurity Internship Program, using PDF files provided by the instructor for this exercise. No unauthorized access or password cracking was performed against any external or third-party system.

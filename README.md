🕒 Encryption-Based Time Verification in Digital Forensics

This repository documents my graduation project at the British Columbia Institute of Technology (BCIT), which explores the use of encryption using VeraCrypt as an indirect method for timestamp verification in digital forensic investigations.

🔍 Project Summary
Timestamps play a vital role in forensic timelines, but they are vulnerable to tampering. This project investigates how encryption artifacts, generated through the use of VeraCrypt, can provide reliable metadata that supports or challenges forensic time analysis. By correlating encryption states with system logs and timestamps, this project aims to enhance time-based evidence verification.

🧪 Methodology
The project was conducted on a DELL Inspiron 15 (Intel Core i7-4510U CPU), using a controlled sequence of forensic imaging and encryption operations:
---Experiment Stages:
1. **Baseline Image**: A clean snapshot before changes.
2. **Image with Timestamp Changes**: Manual changes made using Attribute Changer.
3. **Mid-Encryption Image**: Captured during encryption of a VeraCrypt container.
4. **Fully Encrypted Image**: After full container encryption.
5. **Decrypted Image**:  After decrypting the container.

--- Tools Used:
- **VeraCrypt**: For container encryption/decryption
- **FTK (Forensic Toolkit)**: To extract and analyze file system artifacts
- **Magnet AXIOM**:  For timeline visualization and artifact correlation
- **Attribute Changer**: To simulate manipulated timestamps
- **Windows Event Viewer**:  For log correlation

🔧 Environment and Setup
- VeraCrypt containers were created instead of whole disk encryption to enable live acquisition.
- Timestamps were collected from file metadata, Event Logs, and VeraCrypt volume activity.
- Forensic images were acquired using industry-standard tools and best practices to maintain integrity.

🧠 Key Insights
- VeraCrypt volume creation and mount actions leave system-level traces and timestamps that are resistant to standard tampering.
- Changes in container metadata (e.g., volume headers, mount logs) offer reliable markers for verifying event timelines.
- Encryption artifacts can supplement other forensic evidence in cases involving manipulated timestamps or anti-forensic measures.

👩‍💻 About the Author
**Hareem Fatima**  
Cybersecurity & Digital Forensics Graduate Student  
Bachelor of Technology in Forensic Investigation  
British Columbia Institute of Technology (2023–2025)



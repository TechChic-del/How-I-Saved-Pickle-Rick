# How-I-Saved-Pickle-Rick
# 🥒 How I *Almost* Saved Pickle Rick  
*A TryHackMe Writeup by me 💻*

---

## 🧠 Box Summary
- **Box Name:** Pickle Rick  
- **Goal:** Gain shell access + retrieve 3 secret ingredients  
- **Status:** Accessed web portal, discovered hidden files, ran out of time 😭

---

## ⚙️ Recon Phase

### 🔍 Nmap Scan  
```bash
nmap -sV -A -T4 [IP]
📌 Ports Discovered:
22 → OpenSSH

80 → Apache Web Server

🌐 Web Enumeration:
Visited http://[IP] and found:

/login.php

/robots.txt revealing hidden file

Username (R1ckRul3s) hidden in page source 👀

🔓 Login Bypass
🎯 Credentials Discovered:
Username: R1ckRul3s

Password: Wubbalubbadubdub

✅ Result:
Successfully logged into the portal

Found hidden file: Sup3rS3cretPickl3Ingred.txt

🧾 Unfortunately, couldn't grab screenshots due to time crunch — note for next time!

🧪 Lessons Learned
🕓 Timing is critical in CTFs — every minute counts

🔁 Basic recon (robots.txt, HTML comments) is often all you need to get started

🧱 Next step would’ve been privilege escalation — will revisit this box soon

💡 Final Thoughts:
This box was beginner-friendly and helped sharpen my recon skills. Even though I couldn’t finish it 100%, it was a valuable run.

Stay tuned for my rematch with Pickle Rick 💪

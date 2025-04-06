
# 🛡️ Linux Forensic Toolkit

A Bash-based forensic toolkit developed by **Danielle Taylor** (`Taylortx0316`) as part of a cybersecurity Capstone project. This tool is designed for incident response and malware investigation on Linux systems.

The toolkit automates suspicious behavior detection using:

- ✅ [LinPEAS](https://github.com/carlospolop/PEASS-ng)
- ✅ ClamAV malware scanning
- ✅ Cron, user, and `/tmp` file analysis
- ✅ Interactive CLI menu with modular options
- ✅ Auto-generated forensic report

---

## 📂 Features

- 🔍 Automated LinPEAS execution and keyword filtering
- 🧪 ClamAV signature-based malware scans
- 📅 Monitors for new cron jobs and recent edits
- 🔐 Detects new users and `/etc/shadow` hash changes
- 🧾 Collects and hashes recent `/tmp` file activity
- 📑 Summary report saved to timestamped folder

---

## 📥 Installation

Clone the repo and make the script executable:

```bash
git clone https://github.com/Taylortx0316/linux-forensic-toolkit.git
cd linux-forensic-toolkit
chmod +x linpeas_malware_toolkit.sh

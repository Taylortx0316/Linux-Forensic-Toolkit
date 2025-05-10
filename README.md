AutoThreatScan Toolkit

AutoThreatScan is an automated toolkit for performing deep forensic analysis and malware detection on Linux-based systems. It integrates network scanning, cron job monitoring, /tmp directory monitoring, user forensics, ClamAV scanning, and summary reporting.

📌 Features

Network Analysis: Collects IP information, active connections, and listening ports.

Cron Job Monitoring: Logs user and system cron jobs.

/tmp Directory Monitoring: Detects new files and generates SHA-256 hashes.

User & Password Forensics: Captures information from /etc/passwd and /etc/shadow.

ClamAV Malware Scan: Scans specified directories for malware.

Summary Report Generation: Compiles all logs into a structured report.

🛠️ Installation

# Clone the repository
git clone https://github.com/your-username/AutoThreatScan.git
cd AutoThreatScan

# Make the script executable
chmod +x linpeas_malware_toolkit_final.sh

# Run the script with sudo
sudo bash linpeas_malware_toolkit_final.sh

🚀 Usage

When the script is executed, you will be presented with the following options:

==== LinPEAS Malware Toolkit ====
1) Network Analysis
2) Cron Job Monitoring
3) Monitor /tmp Directory
4) User & Password Forensics
5) ClamAV Malware Scan
6) Generate Summary Report
7) Exit

Select the desired option to perform a scan or generate a report. All logs are stored in /var/log/AutoThreatScan.

📂 Log File Locations

Log Type

File Location

Network Analysis Logs

/var/log/AutoThreatScan/network_logs.log

Cron Job Monitoring Logs

/var/log/AutoThreatScan/cron_changes.log

/tmp Directory Monitoring

/var/log/AutoThreatScan/tmp_new_files.txt

File Hashes

/var/log/AutoThreatScan/tmp_hashes.txt

User & Password Forensics

/var/log/AutoThreatScan/user_monitor.log

ClamAV Malware Scan

/var/log/AutoThreatScan/clamav_scan.txt

Summary Report

/var/log/AutoThreatScan/summary_report.txt

🔍 Future Improvements

Implement real-time monitoring with inotify for /tmp.

Add Splunk integration for advanced analytics.

Schedule automatic runs with cron jobs.

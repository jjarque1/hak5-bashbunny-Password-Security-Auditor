# Password Security Auditor

---

## Description

The **Password Security Auditor** payload is designed to perform a basic audit of password security on a Windows system. It checks for weak or default passwords on key system accounts, such as the administrator and guest accounts. This payload helps in identifying potential vulnerabilities related to password policies and provides a simple way to ensure password security.

## How it Works

1. The payload opens PowerShell with administrator privileges.
2. It checks for weak or default passwords by querying key accounts (e.g., administrator and guest).
3. The results, including password change dates and account details, are saved to a log file.
4. The log file is copied to the Bash Bunny’s storage for later review.

## Requirements

- Target: Windows machine
- Bash Bunny in HID and storage mode

## Ethical Use Disclaimer

This payload is intended for ethical hacking and educational purposes only. Unauthorized password auditing or system access is illegal and unethical. Ensure you have proper authorization before running this script.

## Liability Disclaimer

The author of this payload assumes no responsibility for any illegal or unethical use of the code. This payload is provided as-is, and it is the user's responsibility to ensure its use complies with all applicable laws and regulations.

## Usage

1. Insert the Bash Bunny into the target machine.
2. The payload will automatically perform a password security audit, focusing on key accounts like administrator and guest.
3. The audit results will be saved in `/password_audit.txt` on the Bash Bunny’s storage.
4. Eject the Bash Bunny and review the log file for potential security issues.

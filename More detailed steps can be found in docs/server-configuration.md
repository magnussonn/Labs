
---

### 📜 `scripts/setup.sh` (Install Apache and enable SSH)
```bash
#!/bin/bash
sudo yum update -y
sudo yum install -y httpd openssh-server
sudo systemctl enable httpd
sudo systemctl start httpd
sudo systemctl enable sshd
sudo systemctl start sshd

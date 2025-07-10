# ✅ README.md

## Git Installation Automation Project

This project automates the installation of Git across multiple operating systems using Bash, Python, and Ansible. It is designed to be scalable, production-ready, and auditable.

### 🔧 Tools & Technologies:
- Bash (for initial scripting)
- Python (cross-platform scripting with logging)
- Ansible (infrastructure-wide deployment)
- Jenkins (optional integration)
- AWS EC2

---
## 🗂️ Project Structure

```bash
GITINSTALLATIONPROJECT/
├── README.md
├── bash/
│   └── git_install.sh
├── python/
│   └── git_installer.py
├── ansible/
│   ├── inventory.ini
│   ├── git_install_playbook.yml
│   └── roles/
│       └── git_install/
│           ├── tasks/
│           │   └── main.yml
│           └── defaults/
│               └── main.yml
└── jenkins/
    └── Jenkinsfile
    
## 🧱 Structure Breakdown

### 1. `bash/git_install.sh`
A basic Bash script to detect OS and install Git with minimal dependencies.

### 2. `python/git_installer.py`
A more advanced cross-platform script using Python with structured logging and error handling.

### 3. `ansible/git_install_playbook.yml`
Deploy Git across multiple servers using Ansible. Includes OS detection, idempotency, and logging.

### 4. `jenkins/Jenkinsfile`
(Optional) Jenkins pipeline to trigger the Ansible playbook automatically.

---

## ✅ Usage

### Bash:
```bash
bash bash/git_install.sh
```

### Python:
```bash
python3 python/git_installer.py
```

### Ansible:
```bash
ansible-playbook -i ansible/inventory.ini ansible/git_install_playbook.yml
```

---

## 📌 Real-World Use Case
This was used in a production environment to deploy Git across 30+ AWS EC2 instances using Ansible, with centralized logging and secure provisioning.

---

## 👤 Author
**Vaishnavi Buradkar**

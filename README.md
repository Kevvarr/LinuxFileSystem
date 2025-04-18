# LinuxFileSystem
Linux File System
![hN4lt](https://miro.medium.com/v2/resize:fit:1372/0*X34tDynHLvheJOKN)

## 🔧 System Configuration Files

| File Path | Description |
|-----------|-------------|
| `/etc/passwd` | User account information (usernames, UID, shell). |
| `/etc/shadow` | Encrypted user passwords and password aging. |
| `/etc/group` | Group definitions. |
| `/etc/sudoers` | Sudo access configuration (`visudo` is recommended). |
| `/etc/hostname` | Defines the system's hostname. |
| `/etc/hosts` | Static hostnames to IP mappings. |
| `/etc/fstab` | Filesystem mount table (auto mounts on boot). |
| `/etc/*release` | OS information. |
| `~/.bashrc` | Customize PATH, environment variables, aliases, etc (`source ~/.bashrc` to restart)

---

## 🌐 Networking Files

| File Path | Description |
|-----------|-------------|
| `/etc/network/interfaces` | (Debian/Ubuntu < 18.04) Network interfaces config. |
| `/etc/netplan/*.yaml` | (Ubuntu 18.04+) Netplan YAML network config. |
| `/etc/resolv.conf` | DNS resolver configuration. |
| `/etc/hosts.allow` / `/etc/hosts.deny` | TCP wrapper access control. |
| `/etc/ssh/sshd_config` | SSH daemon configuration (port, auth method, etc). |

---

## 🔐 Security & Access Control

| File Path | Description |
|-----------|-------------|
| `/etc/pam.d/` | Directory for PAM (Pluggable Authentication Modules). |
| `/etc/securetty` | TTYs from which root can login. |
| `/etc/ssh/sshd_config` | Repeated: critical for SSH hardening. |
| `/etc/login.defs` | Default values for user account settings (e.g., password expiration). |

---

## 🗃️ Log Files (Monitoring & Auditing)

| File Path | Description |
|-----------|-------------|
| `/var/log/syslog` | General system activity log (Debian/Ubuntu). |
| `/var/log/messages` | General system activity log (RHEL/CentOS). |
| `/var/log/auth.log` | Authentication attempts and sudo access logs. |
| `/var/log/dmesg` | Kernel ring buffer messages. |
| `/var/log/cron` | Cron job execution log. |
| `/var/log/nginx/access.log` / `error.log` | NGINX logs. |
| `/var/log/httpd/` | Apache web server logs. |

---

## 📦 Package Management Files

| File Path | Description |
|-----------|-------------|
| `/etc/apt/sources.list` | APT repositories list (Debian/Ubuntu). |
| `/etc/yum.repos.d/*.repo` | YUM/DNF repository configs (RHEL/CentOS/Fedora). |

---

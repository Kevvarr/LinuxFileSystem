# LinuxFileSystem
Linux File System
![hN4lt](https://github.com/user-attachments/assets/8119bca3-ac51-4b90-9b76-397c84a9c4ed)

# 🅰️ Essential Apache HTTP Server Files

Apache (httpd) is a widely-used open-source web server. Here are the key files and directories DevOps engineers should know:

---

## 🔧 Configuration Files

| File Path | Description |
|-----------|-------------|
| `/etc/httpd/conf/httpd.conf` | Main Apache config file (RHEL/CentOS). |
| `/etc/apache2/apache2.conf` | Main config (Debian/Ubuntu). |
| `/etc/apache2/envvars` | Environment variables for Apache processes. |
| `/etc/apache2/ports.conf` | Configures which ports Apache listens on. |
| `/etc/apache2/sites-available/` | Virtual host definitions (not active by default). |
| `/etc/apache2/sites-enabled/` | Symlinks to active virtual hosts. |
| `/etc/httpd/conf.d/*.conf` | Additional config files loaded automatically (RHEL/CentOS). |

---

## 📁 Modules

| File/Dir | Description |
|----------|-------------|
| `/etc/httpd/modules/` | Compiled Apache modules (RHEL/CentOS). |
| `/etc/apache2/mods-available/` | Available modules (Debian/Ubuntu). |
| `/etc/apache2/mods-enabled/` | Symlinks to enabled modules. |

---

## 🗃️ Log Files

| File Path | Description |
|-----------|-------------|
| `/var/log/httpd/access_log` | Access logs (RHEL/CentOS). |
| `/var/log/httpd/error_log` | Error logs (RHEL/CentOS). |
| `/var/log/apache2/access.log` | Access logs (Debian/Ubuntu). |
| `/var/log/apache2/error.log` | Error logs (Debian/Ubuntu). |

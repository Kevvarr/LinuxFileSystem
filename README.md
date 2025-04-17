# LinuxFileSystem
Linux File System
![hN4lt](https://github.com/user-attachments/assets/8119bca3-ac51-4b90-9b76-397c84a9c4ed)

# 🅽 Essential NGINX Files for DevOps Engineers

NGINX is a high-performance web server, reverse proxy, and load balancer. Below are the most important config and log files to know.

---

## 🔧 Configuration Files

| File Path | Description |
|-----------|-------------|
| `/etc/nginx/nginx.conf` | Main NGINX configuration file. |
| `/etc/nginx/conf.d/` | Directory for site or service-specific config files. |
| `/etc/nginx/sites-available/` | Site definitions (not active by default). |
| `/etc/nginx/sites-enabled/` | Symlinks to active site configurations. |
| `/etc/nginx/mime.types` | MIME type mappings. |

> On many distributions, only `nginx.conf` and `conf.d/` are used by default. The `sites-*` structure is popular in Ubuntu but not standard in all systems.

---

## 🗃️ Log Files

| File Path | Description |
|-----------|-------------|
| `/var/log/nginx/access.log` | Access logs for served requests. |
| `/var/log/nginx/error.log` | Error logs and startup/shutdown events. |

---

## ✅ Useful Commands

```bash
# Check config syntax
nginx -t

# Reload configuration without downtime
nginx -s reload

# Start / stop / restart NGINX
systemctl start nginx
systemctl stop nginx
systemctl restart nginx

# View active NGINX processes
ps aux | grep nginx

# Always validate config before reloading
nginx -t && systemctl reload nginx

# Experiment 8 - Control the Status of Services Using System Service Commands

## Aim
To learn how to manage and monitor system services in Linux using the `systemctl` command.

---

## Commands

### 1. View the running status of the network service

```bash
sudo systemctl status NetworkManager
```

> If your system uses a different network service:

```bash
sudo systemctl status networking
```

---

### 2. Start, Stop, and Restart a Service

Start a service:

```bash
sudo systemctl start apache2
```

Stop a service:

```bash
sudo systemctl stop apache2
```

Restart a service:

```bash
sudo systemctl restart apache2
```

Check its status:

```bash
sudo systemctl status apache2
```

---

### 3. Restart the Nginx Service

```bash
sudo systemctl restart nginx
```

Verify:

```bash
sudo systemctl status nginx
```

---

### 4. Check the Status of the SSH Service

```bash
sudo systemctl status ssh
```

On some Linux distributions:

```bash
sudo systemctl status sshd
```

---

### 5. Restart the DNS Resolver Service

Ubuntu:

```bash
sudo systemctl restart systemd-resolved
sudo systemctl status systemd-resolved
```

---

## Common systemctl Commands

| Command | Description |
|---------|-------------|
| `systemctl start <service>` | Starts a service |
| `systemctl stop <service>` | Stops a service |
| `systemctl restart <service>` | Restarts a service |
| `systemctl status <service>` | Displays service status |
| `systemctl enable <service>` | Enables service at boot |
| `systemctl disable <service>` | Disables service at boot |

---

## Result

Successfully performed service management operations using the `systemctl` command, including checking service status, starting, stopping, restarting, and managing system services in Linux.

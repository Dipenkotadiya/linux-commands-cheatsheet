# Networking Solutions

### Exercise 1 – Display network interfaces
```bash
ip addr

```

**Output:**

```
2: eth0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 9001 ...
    inet 172.31.19.57/20 brd 172.31.31.255 scope global dynamic eth0

```

✅ The IP address is `172.31.19.57`.

---

### Exercise 2 – Ping google.com

```bash
ping google.com -c 4

```

**Output:**

```
4 packets transmitted, 0 received, 100% packet loss, time 3066ms

```

❌ No packets received → network or DNS issue.

---

### Exercise 3 – Find open ports

```bash
ss -tuln

```

**Output:**

```
tcp LISTEN 0 128 0.0.0.0:22 ...

```

✅ SSH is listening on port 22.

---

### Exercise 4 – Fetch HTTP headers

```bash
curl -I https://www.google.com

```

**Output:**

```
curl: (28) Failed to connect to www.google.com port 443: Connection timed out

```

❌ Unable to connect → network problem or firewall blocking.

---

### Additional Notes:

- The `traceroute` command was not installed by default.
- Installed using:

```bash
sudo apt update
sudo apt install traceroute

```

However, the installation failed because the package repository was unreachable.

```

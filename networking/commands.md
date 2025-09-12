# Networking Commands

### 1. `ss -tuln`
```bash
ss -tuln

```

Lists all listening and non-listening sockets (TCP and UDP), without resolving names.

**Example output explanation:**

- `tcp LISTEN 0 128 0.0.0.0:22` → SSH server is listening on all interfaces at port 22.
- `udp UNCONN 0 0 127.0.0.53:53` → Local DNS resolver listening on loopback.

---

### 2. `ping google.com -c 4`

```bash
ping google.com -c 4

```

Sends 4 ICMP echo requests to `google.com` and shows the round-trip time and packet loss.

**Example output explanation:**

- `4 packets transmitted, 0 received, 100% packet loss` → Network or DNS issue.

---

### 3. `traceroute google.com`

```bash
traceroute google.com

```

Traces the route packets take to reach `google.com`.

**Note:** If not installed, use:

```bash
sudo apt update
sudo apt install traceroute

```

---

### 4. `curl -I https://www.google.com`

```bash
curl -I https://www.google.com

```

Fetches HTTP headers from the specified URL.

**Example output explanation:**

- `HTTP/1.1 200 OK` → Successful connection.
- `Connection timed out` → Server unreachable or network issue.

---

### 5. `ip addr`

```bash
ip addr

```

Displays all network interfaces with their IP addresses.

**Example output explanation:**

- `inet 172.31.19.57/20` → IP address assigned to the interface.
- `lo` → Loopback interface, used internally by the system.

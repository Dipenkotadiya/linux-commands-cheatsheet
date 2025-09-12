# Networking Practice Exercises

1. **Display network interfaces and note their IP addresses.**
   - Use the `ip addr` command and identify your public and private IP.

2. **Ping google.com and record round-trip time.**
   - Run `ping google.com -c 4` and note if packets are lost or the average time.

3. **Find open ports and associated services.**
   - Run `ss -tuln` and find services like SSH or DNS listening on specific ports.

4. **Fetch HTTP headers from a website.**
   - Run `curl -I https://www.google.com` or `curl -I https://www.example.com` and check the HTTP response code.

Commands and what they do

1. ip a: shows all network interfaces and their assigned IP addresses.

Look for inet 10.0.2.15/24 under an interface.

2. ip route: shows the routing table, specifically your default gateway.

Look for the line starting with default via — that's your gateway address.

3. ping -c: tests connectivity to a host, with -c limiting how many pings are sent.

4. curl: fetches content from a URL directly in the terminal.

5. curl -I: fetches only the HTTP headers, not the full page content.

What each character means -I = capital I, requests just the response headers — useful for a quick check of whether a site is up and what server it's running, without downloading the whole page.

6. wget: downloads a file from a URL

7. netstat -tulnp: shows listening network ports and the programs using them.

What character means  -t = TCP, -u = UDP, -l = listening only, -n = numeric (don't resolve names), -p = show the program name.

8. ss -tulnp: the modern replacement for netstat, same flags, same purpose.

9. hostname: shows your machine's current hostname.

10. hostnamectl: shows detailed system identity info, including hostname, OS, and kernel version.

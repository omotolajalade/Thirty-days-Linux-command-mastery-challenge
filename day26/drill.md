Day 26 drill:Identify your machine's IP address and default gateway, test connectivity to a public host, fetch a
URL's headers only, and list every port currently listening. 

ip a                        ← find your IP address
ip route                    ← find your default gateway
ping -c 4 8.8.8.8            ← test connectivity to a public host
curl -I https://example.com  ← fetch headers only
sudo ss -tulnp               ← list every listening port
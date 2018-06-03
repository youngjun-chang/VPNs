# VPN & datacenter IPs
This is a list of common VPN providers. There are lots of lists of open proxies and tor nodes on the web, but surprisingly few usable ones dedicated to VPN providers and datacenters. This list is made up of both known VPN hostnames, and the datacenter IP ranges they're likely to be hosted on. It doesn't list _all_ VPNs because that's obviously impossible, but it should list most common ones.

# Use cases
There are many very legitimate reasons to use VPNs, such as increased privacy. I use a VPN myself, and have recommended the same thing to many people. Still, you may want to block VPNs, or just treat VPNs differently if, for example:

  - You are a game server (especially one that can only ban players by easily changable IPs)
  - You run a commercial application with a very high fraud risk
  - You are Netflix

# How to use
Feed the vpn-ipv4.txt file and/or the vpn-ipv6.txt file to your firewall or application. Ignore the 'source' folder.

For extra effectiveness, you should probably be supplementing this with blocklists for recently abusive IPs, as these invariably include many VPNs, and lists of open proxies/tor nodes. You should be able to find everything you need in that regard at http://iplists.firehol.org. At the very least, consider using _firehol_level1_, _firehol_level2_, _firehol_abusers_1d_, and _firehol_proxies_ with this list, depending on your needs.

# How to contribute
The vpn-ipv4.txt & vpn-ipv6.txt files are distilled from the files in the 'source' folder. I usually  do that manually every two months - being mostly datacenter IPs, these change fairly infrequently. Pull requests are welcome, but you should probably not be modifying vpn-ipv4.txt or vpn-ipv6.txt directly unless there's a blatant error in it. Prefer editing files in the 'source' folder when you can.

# Caveats
This list indiscriminately lists VPNs and datacenters. It may list your own server's IP range, or that of your DNS server, or legitimate search engines. It may eat your children and kidnap your dog. Before implementing, take a moment to make sure you really, definitely want to be doing whatever it is you're doing with this list.

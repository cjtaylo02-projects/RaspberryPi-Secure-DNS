# RaspberryPi-Secure-DNS
Configured a Raspberry Pi Model 4 into a secure at-home DNS server.

## Overview
This project demonstrates how to deploy and secure a home DNS infrastructure that enhances both privacy and network performance. A Raspberry Pi was imaged with Raspberry Pi OS 64-bit, then configured with Pi-hole to block ads and malicious domains network-wide. To prevent DNS hijacking, Unbound was implemented as a recursive DNS resolver, encrypting DNS traffic and validating queries via DNSSEC.

## Key Tasks
- Installed and configured Pi-hole for local DNS resolution and ad-blocking.
- Set up Unbound as a recursive DNS resolver with DNSSEC validation for authenticity.
- Enabled Cloudflared to support DNS-over-HTTPS as a fallback encrypted channel.
- Reserved a static IP through the router and restricted DNS access to LAN-only clients.
- Automated system updates and Pi-hole gravity list refreshes via custom Bash scripts.
- Verified proper query flow and encryption using dig and Pi-hole query logs.
## Tools and Skills
Hardware: Raspberry Pi Model 4 (4GB RAM)
Software: Raspberry Pi OS (64-bit), Pi-hole, Unbound, Cloudflared
Languages / Tools: Bash scripting, Linux CLI, systemd configuration, DHCP/DNS management
## Results
Achieved a fully encrypted, ad-free DNS infrastructure for all devices on the home network. Improved query response time by caching local DNS lookups through Unbound. Reduced external DNS dependency and exposure to third-party logging. Gained hands-on experience configuring secure network services and automating updates in Linux.

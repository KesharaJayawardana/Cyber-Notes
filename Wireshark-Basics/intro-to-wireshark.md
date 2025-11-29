# Wireshark Basics

## What is Wireshark?
- Wireshark is a network protocol analyzer that captures and shows packets on a network interface.
- Use it for troubleshooting, learning protocols, and examining traffic. **Only capture traffic you are authorized to.**

## Capturing traffic
- Open Wireshark and choose the network interface (Wi-Fi, Ethernet).
- Click **Start** to begin capture, **Stop** to end.
- Save captures as `.pcap` files.

## Display filters (to narrow view)
- `ip.addr == 192.168.1.5` — show packets to/from that IP  
- `tcp` — show only TCP packets  
- `udp` — show only UDP packets  
- `http` — show HTTP traffic  
- `dns` — show DNS queries/responses

## Capture filters (before capture)
- `host 192.168.1.5` — capture only traffic to/from that host  
- `port 80` — capture only port 80 traffic  
- Capture filters use tcpdump/BPF syntax.

## Common analysis steps
1. Identify top talkers: see “Endpoints” / “Conversations”.  
2. Use display filters to isolate suspicious flows.  
3. Follow TCP stream: right-click packet → **Follow** → **TCP Stream**.  
4. Inspect packet details and hex to find payloads or headers.  
5. Export objects (e.g., HTTP) via `File → Export Objects`.

## Useful tips
- Use short captures first (10–30 seconds).  
- Filter before saving to reduce file size.  
- Save interesting packets as a new pcap for sharing or later analysis.  
- Comment or mark packets in Wireshark for notes.

## Common protocols to look for
- ARP, IP, TCP, UDP, ICMP, DNS, HTTP, HTTPS (encrypted), TLS.

## Ethics and legality
- Only capture traffic on networks you own or have permission to analyze. Unauthorized packet capture is illegal.
  
## Resources
- Official docs: wireshark.org/docs  
- Practice: open pcap files from public repositories (search for sample pcaps)

IPv6
Current Configuration
IPv6 enabled on AT&T BGW320-500.
IPv6 prefix delegation managed by AT&T.
Router Advertisements enabled.
SLAAC enabled.
IPv6 DNS distribution is currently controlled by the gateway.
Pi-hole supports IPv6 DNS queries.
IPv6 DNS usage is currently opt-in rather than enforced network-wide.
Current Raspberry Pi IPv6 Addresses
Address	Purpose
2600:1700:9830:8e50::14/128	ISP-provided IPv6 address
2600:1700:9830:8e50:da3a:ddff:fe61:ba52/64	SLAAC address
fe80::da3a:ddff:fe61:ba52/64	Link-local address

These addresses are dynamically assigned and should not be treated as permanent.

Current DNS Configuration
DNS Server	Address
Pi-hole IPv4	192.168.1.246
Pi-hole IPv6	2600:1700:9830:8e50:da3a:ddff:fe61:ba52
Unbound	127.0.0.1:5335

The Pi-hole IPv6 address is currently used for opt-in client configurations.

Future Improvements
Investigate IPv6 Router Advertisement DNS (RDNSS).
Investigate DHCPv6 DNS distribution.
Evaluate enforcing Pi-hole as the default IPv6 DNS resolver.
Consider introducing a dedicated router/firewall such as OPNsense.
Evaluate stable Unique Local Addresses (ULA).
Avoid relying on dynamically assigned ISP global IPv6 addresses for permanent internal DNS records.
Ensure IPv6 clients cannot unintentionally bypass Pi-hole.

Network-wide IPv6 DNS enforcement is intentionally deferred until the gateway's capabilities and future router architecture are evaluated.

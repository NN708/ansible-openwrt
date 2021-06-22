# nn708.openwrt.wireguard

Install and configure WireGuard VPN.

## Role Variables

Name | Default
--- | ---
openwrt_wireguard_interface_name | vpn
openwrt_wireguard_firewall_zone | lan
openwrt_wireguard_private_key
openwrt_wireguard_listen_port
openwrt_wireguard_addresses
openwrt_wireguard_peers

## References

+ https://openwrt.org/docs/guide-user/services/vpn/wireguard/server
+ https://openwrt.org/docs/guide-user/services/vpn/wireguard/client
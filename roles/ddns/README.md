# nn708.openwrt.ddns

Install and configure dynamic DNS (DDNS) service.

## Role Variables

Name | Default
--- | ---
openwrt_ddns_enabled | 0
openwrt_ddns_lookup_host
openwrt_ddns_domain
openwrt_ddns_username
openwrt_ddns_password
openwrt_ddns_interface
openwrt_ddns_service_name
openwrt_ddns_update_url
openwrt_ddns_update_script
openwrt_ddns_ip_source
openwrt_ddns_ip_network
openwrt_ddns_ip_url
openwrt_ddns_ip_interface
openwrt_ddns_ip_script

There are also variables to specify IPv4 or IPv6 configurations. For example, set `openwrt_ddns_ipv4_enabled` to 1 will only enable DDNS for IPv4.

## References

+ https://openwrt.org/docs/guide-user/base-system/ddns
+ https://openwrt.org/docs/guide-user/services/ddns/client
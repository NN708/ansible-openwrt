# nn708.openwrt.wireless_enterprise

Configure WPA Enterprise Wi-Fi security (802.1X).

## Role Variables

Name | Default
--- | ---
openwrt_wireless_disabled | 0
openwrt_wireless_auth_server
openwrt_wireless_auth_port
openwrt_wireless_auth_secret

There are also variables to specify 2.4GHz or 5GHz configurations. For example, set `openwrt_wireless_2_4g_disabled` to 1 will only disable 2.4GHz Wi-Fi.

## References

+ https://openwrt.org/docs/guide-user/network/wifi/basic#wpa_enterprise_access_point
+ https://openwrt.org/docs/guide-user/network/wifi/wireless.security.8021x
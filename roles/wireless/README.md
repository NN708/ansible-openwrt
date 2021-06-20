# nn708.openwrt.wireless

Configure Wi-Fi settings.

## Role Variables

Name | Default
--- | ---
openwrt_wireless_disabled | 0
openwrt_wireless_channel | auto
openwrt_wireless_country
openwrt_wireless_ssid
openwrt_wireless_encryption
openwrt_wireless_key
openwrt_wireless_hidden
openwrt_wireless_isolate
openwrt_wireless_macfilter
openwrt_wireless_maclist
openwrt_wireless_ieee80211r

There are also variables to specify 2.4GHz or 5GHz configurations. For example, set `openwrt_wireless_2_4g_disabled` to 1 will only disable 2.4GHz Wi-Fi.

## References

+ https://openwrt.org/docs/guide-user/network/wifi/basic
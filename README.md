# Ansible Collection for OpenWrt

Ansible collection to configure your OpenWrt devices more quickly and automatically (without Python).

## Installation

1. [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) should be installed on your control node, but nothing needs to be installed on your OpenWrt devices.

2. This collection depends on `gekmihesg.openwrt`. Install it using

    ```
    ansible-galaxy install gekmihesg.openwrt
    ```

3. Install this collection using

    ```
    ansible-galaxy collection install nn708.openwrt
    ```

## Content

This collection includes these roles:

+ [nn708.openwrt.ddns](https://github.com/NN708/ansible-openwrt/tree/master/roles/ddns)
+ [nn708.openwrt.network](https://github.com/NN708/ansible-openwrt/tree/master/roles/network)
+ [nn708.openwrt.system](https://github.com/NN708/ansible-openwrt/tree/master/roles/system)
+ [nn708.openwrt.wireless](https://github.com/NN708/ansible-openwrt/tree/master/roles/wireless)
+ [nn708.openwrt.wireless_enterprise](https://github.com/NN708/ansible-openwrt/tree/master/roles/wireless_enterprise)

## Example Playbook

This is a minimal working example to set up a basic wireless router:

```yaml
---
- hosts: openwrt

  vars:
    ansible_user: root
    openwrt_network_wan_proto: pppoe
    openwrt_network_wan_username: my-user
    openwrt_network_wan_password: my-passwd
    openwrt_system_zonename: Asia/Shanghai
    openwrt_wireless_country: CN
    openwrt_wireless_ssid: my-wi-fi
    openwrt_wireless_encryption: psk2
    openwrt_wireless_key: my-passwd

  roles:
    - nn708.openwrt.network
    - nn708.openwrt.system
    - nn708.openwrt.wireless
```

> Because of using `gekmihesg.openwrt`, `openwrt` should be used as the group name of hosts. See [gekmihesg/ansible-openwrt#example-playbook](https://github.com/gekmihesg/ansible-openwrt#example-playbook) for example inventory file.

## License

Licensed under [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.txt).
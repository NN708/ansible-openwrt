# Ansible Collection for OpenWrt

Ansible collection to configure your OpenWrt devices more quickly and automatically (without Python).

## Installation

1. This collection depends on `gekmihesg.openwrt`. Install it using

    ```
    ansible-galaxy install gekmihesg.openwrt
    ```

2. Install this collection using

    ```
    ansible-galaxy collection install nn708.openwrt
    ```

## Content

This collection includes these roles:

+ [nn708.openwrt.system](https://github.com/NN708/ansible-openwrt/tree/master/roles/system)
+ [nn708.openwrt.wireless](https://github.com/NN708/ansible-openwrt/tree/master/roles/wireless)
+ [nn708.openwrt.wireless_enterprise](https://github.com/NN708/ansible-openwrt/tree/master/roles/wireless_enterprise)

## Example Playbook

## License

Licensed under [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.txt).
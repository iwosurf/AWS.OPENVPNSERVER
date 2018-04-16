Ansible openvpn server

  * Install OpenVPN server

Variables roles/openvpn/defaults/main.yml

```javascript
# Default networking interface
openvpn_interface: enp0s3
openvpn_path: /etc/openvpn
openvpn_port: 1194
openvpn_proto: udp
openvpn_server_hostname: "{{inventory_hostname}}"
openvpn_use_modern_tls: true
openvpn_resolv_retry: 5
openvpn_client_register_dns: true
openvpn_verify_cn: false
openvpn_fetch_config_dir: /tmp/ansible
```

```javascript
# OpenVpn Server IP
openvpn_server_ip: 10.10.10.1
openvpn_server_subnet: 255.255.255.0
```

# Install settings
openvpn_use_system_easyrsa: false

```javascript
# Default settings certificates
openvpn_etcdir: /etc/openvpn
openvpn_key_dir: /etc/openvpn/keys
openvpn_rsa_bits: 2048
clients: [alpha, omega]
openvpn_base_dir: /etc/openvpn
```

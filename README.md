Ansible openvpn server

  * Install OpenVPN server

Variables

# Default networking interface
openvpn_interface: enp0s3
openvpn_path: /etc/openvpn
openvpn_port: 1194
openvpn_proto: udp

# Install settings
openvpn_use_system_easyrsa: false

# Default settings certificates
openvpn_etcdir: /etc/openvpn
openvpn_keydir: "{{openvpn_etcdir}}/keys"

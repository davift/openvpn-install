

## openvpn-install

![Static Badge](https://img.shields.io/badge/Bash-blue?style=social&logo=gnubash)

OpenVPN [road warrior](http://en.wikipedia.org/wiki/Road_warrior_%28computing%29) installer for Ubuntu, Debian, AlmaLinux, Rocky Linux, CentOS, and Fedora.

This script will let you set up your own VPN server in no more than a minute, even if you haven't used OpenVPN before. It has been designed to be as unobtrusive and universal as possible.

### Installation
Run the script and follow the assistant:

```
wget https://raw.githubusercontent.com/davift/openvpn-install/master/openvpn-install.sh -O openvpn-install.sh && bash openvpn-install.sh
```

Once it ends, you can run it again to add more users, remove some of them, or even completely uninstall OpenVPN.

### Automation
Check out the script `openvpn-cli.sh` for user management with a single command line, easy to integrate into other scripts or with Ansible or Terraform.

If the client name is an email address, `openvpn-cli.sh add` will email the generated `.ovpn` profile via `msmtp`. Set the sender with the `MAIL_FROM` environment variable (defaults to `noreply@<hostname>`).

New: [wireguard-install](https://github.com/Nyr/wireguard-install) is also available.

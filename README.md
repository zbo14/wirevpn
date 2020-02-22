# wirevpn

This project is a continuation of [diy-vpn](https://github.com/zbo14/diy-vpn), which contains instructions and tools to run personal [OpenVPN](https://openvpn.net/) and [WireGuard](https://www.wireguard.com/) VPNs.

I created this repo because (1) I wanted a dedicated project for WireGuard, and (2) I wanted to incorporate wishlist features that were beyond the scope of the original proof-of-concept. I *could* have made these changes to `diy-vpn`, but rather than subject the repo to an indeterminate amount of trial-and-error, I thought it better to experiment in separate repos.

The aforementioned features include:
* Use of pre-shared keys as an additional layer of symmetric encryption (e.g. for post-quantum resistance)
* Encryption of private and pre-shared keys on peer devices
* DNS-over-TLS from VPN server to Quad9/Cloudflare
* Any others? If you have ideas, please [open an issue](https://github.com/zbo14/wirevpn/issues/new)!

`wirevpn` includes a [server](https://github.com/zbo14/wirevpn-server) and a [client](https://github.com/zbo14/wirevpn-client) component.

Each component contains scripts and config files to expedite the installation, setup, deployment, and usage processes.

Both components run on Ubuntu and have been tested on Bionic Beaver (18.04).

You can deploy the server on an Ubuntu VPS from your cloud hosting platform of choice.

You can use the client on your personal devices running Ubuntu. Please refer to [the website](https://www.wireguard.com/install/) for instructions on how to download/install WireGuard on other distros/mobile devices.

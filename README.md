# Libernet
Libernet is open source web app for tunneling internet using SSH, V2Ray on OpenWRT with ease.

## Requirements
- bash
- screen
- jq
- Python 3
- OpenSSH
- sshpass
- stunnel
- V2Ray
- go-tun2socks
- badvpn-tun2socks (legacy)
- php7
- php7-cgi
- php7-mod-session
- php7-mod-json

## Working Features:
- SSH with proxy
- SSH-SSL
- V2Ray trojan
- V2Ray vmess

## Installation
- If you don't have git on OpenWRT, please install first: ```opkg update && opkg install git```
- Prepare installation directory: ```mkdir -p ~/Downloads && cd ~/Downloads```
- Clone this repository: ```git clone git://github.com/lutfailham96/libernet.git```
- Run installation script: ```cd libernet && bash install.sh```
- Open Libernet on http://router-ip/libernet
- Fill your tunnel server, save configuration & run Libernet
- Don't forget to update firewall setting to WAN on interface 'tun1' via Luci

## Updating
- Just run updater script: ```bash update.sh```
- Updater script will updating Libernet to latest version

## Default Username & Password
- Username: admin
- Password: libernet

## Additional Information
In home menu, check 'Use tun2socks legacy' to use badvpn-tun2socks or uncheck to use go-tun2socks instead.

<h2 align="center"> Supported Linux Distribution</h2>
<p align="center">
    <img src="/banner/debub.png" width="500" height="300">
</p>
<p align="center"><img src="https://img.shields.io/static/v1?style=for-the-badge&logo=debian&label=Debian%209&message=Stretch&color=purple"> <img src="https://img.shields.io/static/v1?style=for-the-badge&logo=debian&label=Debian%2010&message=Buster&color=purple"> <img src="https://img.shields.io/static/v1?style=for-the-badge&logo=debian&label=Debian%2011&message=Bullseye&color=purple">
</p>

<p align="center"><img src="https://img.shields.io/static/v1?style=for-the-badge&logo=ubuntu&label=Ubuntu%2018&message=Lts&color=red"> <img src="https://img.shields.io/static/v1?style=for-the-badge&logo=ubuntu&label=Ubuntu%2020&message=Lts&color=red"> <img src="https://img.shields.io/static/v1?style=for-the-badge&logo=ubuntu&label=Ubuntu%2022&message=Lts&color=red">
</p>

<p align="center"><img src="https://img.shields.io/badge/Service-SSH_Over_Websocket-success.svg"> <img src="https://img.shields.io/badge/Service-SSH_UDP_Custom-success.svg"> <img src="https://img.shields.io/badge/Service-SSH_Dropbear-success.svg">  <img src="https://img.shields.io/badge/Service-Stunnel4-success.svg"> <img src="https://img.shields.io/badge/Service-Fail2Ban-brightgreen"> <img src="https://img.shields.io/badge/Service-OpenVPN-brightgreen">
<p align="center"><img src="https://img.shields.io/badge/Service-XRAY_VLESS-success.svg">  <img src="https://img.shields.io/badge/Service-XRAY_VMESS-success.svg">  <img src="https://img.shields.io/badge/Service-XRAY_TROJAN-success.svg"> <img src= "https://img.shields.io/badge/Service-Websocket-success.svg"> <img src= "https://img.shields.io/badge/Service-GRPC-success.svg"> <img src= "https://img.shields.io/badge/Service-Shadowsocks-success.svg">  
<p <p align="center"><img src="https://img.shields.io/badge/Service-Webmin-success.svg"> <img src="https://img.shields.io/badge/Service-Helium-success.svg">
<p <p align="center"><img src="https://wangchujiang.com/sb/status/stable.svg">

## Service & Port:
<table>
  <tr>
    <td>OpenSSH</td>
    <td>:</td>
    <td>22</td>
    <td></td>
    <td>Shadowsocks WS TLS</td>
    <td>:</td>
    <td>443</td>
  </tr>
  <tr>
    <td>SSH Websocket</td>
    <td>:</td>
    <td>80</td>
    <td></td>
    <td>Vmess WS none TLS</td>
    <td>:</td>
    <td>80</td>
  </tr>
  <tr>
    <td>SSH SSL Websocket</td>
    <td>:</td>
    <td>443</td>
    <td></td>
    <td>Vless WS none TLS</td>
    <td>:</td>
    <td>80</td>
  </tr>
  <tr>
    <td>Stunnel4</td>
    <td>:</td>
    <td>222, 777</td>
    <td></td>
    <td>Trojan WS none TLS</td>
    <td>:</td>
    <td>80</td>
  </tr>
  <tr>
    <td>Dropbear</td>
    <td>:</td>
    <td>109, 143</td>
    <td></td>
    <td>Shadowsocks WS none TLS</td>
    <td>:</td>
    <td>80</td>
  </tr>
  <tr>
    <td>Badvpn</td>
    <td>:</td>
    <td>7100-7900</td>
    <td></td>
    <td>Vmess gRPC</td>
    <td>:</td>
    <td>443</td>
  </tr>
  <tr>
    <td>Nginx</td>
    <td>:</td>
    <td>81</td>
    <td></td>
    <td>Vless gRPC</td>
    <td>:</td>
    <td>443</td>
  </tr>
  <tr>
    <td>Vmess WS TLS</td>
    <td>:</td>
    <td>443</td>
    <td></td>
    <td>Trojan gRPC</td>
    <td>:</td>
    <td>443</td>
  </tr>
  <tr>
    <td>Vless WS TLS</td>
    <td>:</td>
    <td>443</td>
    <td></td>
    <td>Shadowsocks gRPC</td>
    <td>:</td>
    <td>443</td>
  </tr>
  <tr>
    <td>Trojan WS TLS</td>
    <td>:</td>
    <td>443</td>
    <td></td>
    <td>Udp-Custom</td>
    <td>:</td>
    <td>1-65535</td>
  </tr>
</table>

# PREVIEW
<p float="left">
  <img src="/preview/pekokepol.jpg" width="32%" />
  <img src="/preview/terk.jpg" width="32%" />
  <img src="/preview/njiai.jpg" width="32%" />
</p>

# CARA INSTALLASI
[ 1 ]  Ganti Repo OS (opsional)
```
#rm /etc/apt/sources.list && nano /etc/apt/sources.list
```
[ 2 ]  Update&Upgrade OS (wajib)
```
apt update && apt upgrade -y && apt install sudo -y && reboot
```
[ 3 ]  Install Dependensi (wajib)
```
sudo apt install dnsutils cron python3 gcc make build-essential zip unzip wget curl screen libz-dev g++ libreadline-dev libreadline-dev zlib1g-dev libssl-dev dos2unix cron vnstat mc jq bzip2 gzip vnstat coreutils rsyslog iftop git apt-transport-https build-essential earlyoom htop iptables jq python2 ruby cmake coreutils rsyslog net-tools nano sed gnupg gnupg1 bc jq dirmngr libxml-parser-perl lsof libsqlite3-dev python3-pip -y && python3 -m pip install --upgrade pip &&  python3 -m pip install tabulate && wget https://github.com/fians-xd/mmk/raw/refs/heads/main/shc.zip && unzip shc.zip && cd shc && sudo chmod +x * && sudo ./configure && sudo make && sudo make install && cd && rm -rf shc.zip shc
```
[ 4 ]  Install-Sc (pasti wajib)
```
wget https://raw.githubusercontent.com/fians-xd/AutoScript.vpn/master/install.sh && chmod +x install.sh && ./install.sh
```

<h2 align="center"> Butuh Bantuan Silahkan DM </h2>
<div align="center">
  <a href="https://wa.me/6287749044636" target="_blank">
    <img src="https://cdn-icons-png.flaticon.com/128/4494/4494494.png" alt="WhatsApp" width="35" height="35" style="vertical-align: middle;"/>
  </a>
  <a href="https://t.me/yansxdi" target="_blank" style="margin-left: 10px;">
    <img src="https://upload.wikimedia.org/wikipedia/commons/8/82/Telegram_logo.svg" alt="Telegram" width="35" height="35" style="vertical-align: middle;"/>
  </a>
</div>

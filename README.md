# Shadowsocks Configuration
## Install Shadowsocks Python Server With Enable BBR On Ubuntu 20.04 LTS
![shadowsocks tunnel proxy server](https://netslovers.com/wp-content/uploads/2022/03/shadowsocks.png)

We will try to install the tunnel proxy Shadowsocks Python Server on our Ubuntu 20.04 LTS, and enable BBR (Bottleneck Bandwidth and RTT) to improve the Linux response time, network speed, and performance, by setting up the system config TCP congestion control to BBR.

The complete turorial url is: https://netslovers.com/2022/03/11/python-pip-install-shadowsocks-with-bbr/


### we will need to:
1. Update our Ubuntu Server
2. Install Python 2.7 and PIP2
3. Install Shadowsocks-Python Server
4. Enable BBR
5. Set Our Server QR Code And Base64 Encoded URI

### Set BBR tcp_congestion_control And Tunning The Kernel For Shadowsocks

Create the file [local.conf](./local.conf) into the sysctl configuration path /etc/sysctl.d/local.conf and insert the following configs
and apply changes by runngin `# sysctl -p`


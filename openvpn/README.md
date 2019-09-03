# Details
A docker-compose file for OpenVPN server. This file consists of 2 OpenVPN containers. One is for UDP connections (which is default) and one is for TCP connections (in order to prevent firewall or proxy blocking). 

You should first initialize OpenVPN and create at least one `.ovpn` certificate. Check the original [OpenVPN](https://github.com/kylemanna/docker-openvpn) repository by [kylemanna](https://github.com/kylemanna) for more information.
# openfirewall (Date : 17 Jun 2026)

Project Plan :

Running on the latest version of OpenWRT (current version 25.12.4)

Support / Target Hardware (Testing device) :
High-End Version (Full version) : x86 (CW-MTL-MINI-4L-PCIe, Ultra 7 155H , 64GB Ram, 2TB SSD)
Standard Version (Standard) : ARM -- GL.inet Flint 2 (if the GL.inet Flint 4 is added to the stable OpenWRT list, we will add it to our list)
Middle Version : Linksys wrt3200acm, wrt32x (will try to support it until the EoL of the latest stable OpenWRT version support)
Travel Version : Glinet Beryl AX (If the Glinet Slate 7 or Slate 7 Pro is added to the stable OpenWRT list, we will add it to our list)

The High-End Version (Full version) x86, will have additional security features!

Planning Tools :
Firewall (ACL) : iptable
Firewall (deep packet inspection) : Netify, nDPI
Firewall (Application Firewall) : Privoxy
HTTPS inspection / WAF : bunkerweb, mitmproxy, nginx-mod-naxsi
IDS/IPS : snort
Gateway Anti-Virus : clamav
DNS / Website Filtering: DNSMASQ
VPN : Open VPN (NordVPN use), Wireguard VPN
Other Tools : tcpdump, iperf3, nginx, USB storage tools


Phase 1 (Now):
Compile the latest version of tools/software/apps
Create the LUCI WebUI for all the apps
Test on Linksys wrt3200acm

Phase 2 :
Compile the tools for : Glinet Beryl AX, GL.inet Flint 2 (If other GL.inet routers officially support the native OpenWRT, they will also be added to the list)

Phase 3 : 
Compile the OpenWRT firmware with all the tools in a single bin file for OpenWRT firmware upgrade.

Phase 4 :
Setup the automation

Phase 5 : 
Design the new Web UI for the openfirewall.

Phase 6 :
Develop the x86 version

Phase 7 :
Develop the add-on feature for the x86 version

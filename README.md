# openfirewall (Date : 17 Jun 2026)<br>
<br>
Project Plan :<br>
<br>
Running on the latest version of OpenWRT (current version 25.12.4)<br>
<br>
Support / Target Hardware (Testing device) :<br>
High-End Version (Full version) : x86 (CW-MTL-MINI-4L-PCIe, Ultra 7 155H , 64GB Ram, 2TB SSD)<br>
Standard Version (Standard) : ARM -- GL.inet Flint 2 (if the GL.inet Flint 4 is added to the stable OpenWRT list, we will add it to our list)<br>
Middle Version : Linksys wrt3200acm, wrt32x (will try to support it until the EoL of the latest stable OpenWRT version support)<br>
Travel Version : Glinet Beryl AX (If the Glinet Slate 7 or Slate 7 Pro is added to the stable OpenWRT list, we will add it to our list)<br>
<br>
The High-End Version (Full version) x86, will have additional security features!<br>
<br>
Planning Tools :<br>
Firewall (ACL) : iptable<br>
Firewall (deep packet inspection) : Netify, nDPI<br>
Firewall (Application Firewall) : Privoxy<br>
HTTPS inspection / WAF : bunkerweb, mitmproxy, nginx-mod-naxsi<br>
IDS/IPS : snort<br>
Gateway Anti-Virus : clamav<br>
DNS / Website Filtering: DNSMASQ<br>
VPN : Open VPN (NordVPN use), Wireguard VPN<br>
Other Tools : tcpdump, iperf3, nginx, USB storage tools<br>
<br>
<br>
Phase 1 (Now):<br>
Compile the latest version of tools/software/apps<br>
Create the LUCI WebUI for all the apps<br>
Test on Linksys wrt3200acm and GLinet Flint 2<br>
<br>
Phase 1 software lists :<br>
- Snort -- done<br>
- nDpi/Netify - WIP<br>
- clamav - WIP re-design<br>
- WAF : bunkerweb, mitmproxy, nginx-mod-naxsi -- wip<br>
<br>
Phase 2 :<br>
Compile the tools for : Glinet Beryl AX, GL.inet Flint 2 (If other GL.inet routers officially support the native OpenWRT, they will also be added to the list)<br>
<br>
Phase 3 : <br>
Compile the OpenWRT firmware with all the tools in a single bin file for OpenWRT firmware upgrade.<br><br>
<br>
Phase 4 :<br>
Setup the automation<br><br>
<br>
Phase 5 : <br>
Design the new Web UI for the openfirewall.<br>
<br>
Phase 6 :<br>
Develop the x86 version<br>
<br>
Phase 7 :<br>
Develop the add-on feature for the x86 version<br>

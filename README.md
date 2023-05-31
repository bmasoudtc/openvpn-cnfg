# openvpn-cnfg
configure a Windows Server 2012 for running OpenVPN

1- Install OpenVPN: The first step is to download and install OpenVPN on your Windows Server. You can download the latest version of OpenVPN from the official website.

2- Configure firewall rules: OpenVPN requires several ports to be open in your firewall. You need to create inbound and outbound rules in Windows Firewall for the following ports: UDP 1194 (for OpenVPN), TCP 443 (for HTTPS), and ICMP (for ping).

3- Generate certificates: OpenVPN requires digital certificates to authenticate clients and servers. You can use the EasyRSA script included with OpenVPN to generate these certificates.

4- Edit the server configuration file: Once OpenVPN is installed and certificates are generated, you need to edit the server configuration file. The default location for this file is C:\Program Files\OpenVPN\config\server.ovpn. You can use any text editor to edit this file.

5- Start OpenVPN service: After editing the server configuration file, start the OpenVPN service by running the "openvpn.exe" command with the server configuration file as an argument.

6- Create client configuration files: The last step is to create client configuration files for each client that will connect to the OpenVPN server. These files should include the client certificate and key, as well as the IP address and port of the OpenVPN server.

That's it! With these steps, you should now have a configured Windows Server 2012 ready to run OpenVPN.

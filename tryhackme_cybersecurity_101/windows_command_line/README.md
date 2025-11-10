# Windows CMD Essentials

## Essentials Commands

- ipconfig /all - This command can be used to list all the network information on the system. Terminal output will display the IP address, Subnet Mask, Default Gateway, and DNS Servers.
  
- Systeminfo - This command is used to list various information about the system, system details, processor and memory.
  
- nslookup - It can be used to find information about a website's IP address by using the website's Domain Name. As an example, nslookup example.com
  
- netstat - This command displays the current network connections(established connections) and listening ports.
  
- netstat -abon - This helps to see all the information of the connections, whether the connection is established or listening, it displays the local IP address and the foreign IP address, and also the type of the connection (TCP or UDP) and ports.
1. This command is useful for identifying suspicious connections, such as malware or unknown apps
2. Open ports can be an attacker's entry points, netstat helps us to see which are open and what they are using them.
   

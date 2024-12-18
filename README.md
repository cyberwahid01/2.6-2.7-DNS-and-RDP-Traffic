<p align="center">
<img src="https://imgur.com/wYucC7L.png" alt="osTicket logo"/>
</p>

<h1>Microsoft Azure Compute and Networking 🪟 - Observe DNS (Domain Name System) and RDP (Remote Desktop Protocol) Traffic</h1>
In this section I use the DNS and RDP Protocols to observe traffic using Wireshark <br />

<h2>Environments and Technologies Used</h2>

- Lenovo Ideapad 5 Pro 16gb AMD Ryzen 7
- Microsoft Azure Resource Group (from [Part 1 - Setting Up Virtual Machines](https://github.com/cyberwahid01/2.1-Virtual-Machine-Setup))
- Microsoft Azure Windows 10 Pro version 22H2 - x64 Gen2 Virtual Machine (from [Part 1 - Setting Up Virtual Machines](https://github.com/cyberwahid01/2.1-Virtual-Machine-Setup))
- Microsoft Azure Ubuntu Pro 24.04 LTS - x64 Gen2 Virtual Machine (from [Part 1 - Setting Up Virtual Machines](https://github.com/cyberwahid01/2.1-Virtual-Machine-Setup))
- Wireshark Network Protocol Analyzer Software
- Windows Powershell

<h2>Operating Systems Used </h2>

- Local Windows 11 Home Version 21H2</b>
- Windows 10 Pro version 22H2 Virtual Machine
- Ubuntu Pro 24.04 LTS - x64 Gen2 Virtual Machine

<h2>List of Prerequisites</h2>

- Microsoft Azure Subscription
- Microsoft Azure Subsription Credit
- Wireshark Installed on Windows 10 Virtual Machine

<h2>Installation, Setup, Resource Setup, Executing Functions</h2>

1. I started off initialising packet capture within Wireshark and filtered for DNS traffic.
<p>
<img src="https://imgur.com/67kkrGc.png" alt="Disk Sanitization Steps"/>
</p>
<p>
2. I then used the command nslookup to obtain the IP address of google.com which we can see was obtained to be 142.250.178.14.
</p>
<br />

<p>
<img src="https://imgur.com/dkviLEc.png" alt="Disk Sanitization Steps"/>
</p>
<p>
3. At this stage I filtered the packet capture traffic using tcp.port == 3389 which shows the traffic over the RDP protocol. Here there is constant traffic because data is always being transmitted between our two Virutal Machines.
</p>
<br />

<p>
<img src="https://imgur.com/BC3HUte.png" alt="Disk Sanitization Steps"/>
</p>
<p>

Cybersecurity Testing Lab Setup using VirtualBox and Kali Linux
1. Project Overview
This project focuses on setting up a basic Cybersecurity Testing Lab using Oracle VirtualBox and Kali Linux.
Kali Linux is configured as the attacking machine for learning cybersecurity and ethical hacking concepts in a controlled virtual environment.
2. Tools and Technologies Used
Oracle VirtualBox
Kali Linux
7-Zip
NAT Network
Linux Terminal
3. Lab Requirements
Install the latest recommended version of VirtualBox.
Set up Kali Linux as the attacking machine.
Configure the network using the 10.0.0.0/24 subnet.
Create a NAT Network in VirtualBox.
Enable clipboard sharing and drag-and-drop.
Enable shared folders with the host machine's Downloads folder.
Assign Kali Linux the IP address 10.0.0.2/24.
Ensure Kali Linux has internet access.
4. Network Configuration
Configuration
Details
Virtualization Tool
Oracle VirtualBox
Operating System
Kali Linux
Network Type
NAT Network
Network Subnet
10.0.0.0/24
Kali Linux IP
10.0.0.2/24
Default Gateway
10.0.0.1
DNS Server
8.8.8.8
5. Installation Steps
Step 1: Download and install 7-Zip.
https://7-zip.org/download.html
Step 2: Download and install Oracle VirtualBox.
https://virtualbox.org/wiki/Downloads
Step 3: Configure a NAT Network in VirtualBox using the subnet 10.0.0.0/24.
Step 4: Download and import the Kali Linux Virtual Machine.
https://www.kali.org/get-kali/
Step 5: Configure the Kali Linux network settings.
Step 6: Take a snapshot of the virtual machine.
6. Kali Linux Network Configuration Commands
The following commands were used in the Kali Linux terminal to configure the network.
Step 1: Assign IP Address
sudo ip addr add 10.0.0.2/24 dev eth0
Step 2: Enable Network Interface
sudo ip link set eth0 up
Step 3: Check IP Address
ip addr show eth0
Step 4: Configure Default Gateway
sudo ip route add default via 10.0.0.1
Step 5: Verify Routing Table
ip route show
Step 6: Test Gateway Connectivity
ping -c 4 10.0.0.1
Step 7: Test Internet Connectivity
ping -c 4 8.8.8.8
7. Network Troubleshooting
If Kali Linux does not have internet access:
Check whether the NAT Network is created correctly.
Verify the VirtualBox network adapter settings.
Ensure the correct network interface is enabled.
Restart Kali Linux and check the connection.
Verify the IP address and default gateway.
8. Expected Outcome
Kali Linux virtual machine successfully installed.
NAT Network configured with the 10.0.0.0/24 subnet.
Static IP address assigned to Kali Linux.
Default gateway configured.
Network connectivity tested using ping commands.
Internet connectivity verified.
9. Conclusion
Successfully configured a basic Cybersecurity Testing Lab using VirtualBox and Kali Linux. This environment provides a foundation for learning cybersecurity, ethical hacking, and practical network security concepts.
Project Type: Cybersecurity Lab Setup
Platform: VirtualBox
Operating System: Kali Linux
Network: NAT Network

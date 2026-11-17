# Ex. No: 6 Identifying MAC and IP Addresses Using Packet Tracer
# Date:17.11.2026
# Name:Abinaya P
# Register number: 212225230003

________________________________________
# Objective
To use Cisco Packet Tracer simulation mode to capture and analyze MAC and IP address information for both local and remote network communication.
________________________________________
# Apparatus/Tools Required
•	Cisco Packet Tracer<br>
•	Pre-configured network topology (as provided in the activity file)<br>
•	PCs, switches, router, hub, and wireless access point (as per given setup)<br>
________________________________________
# Network Topology Diagram
# Description:
•	The topology contains a local network (172.16.31.0/24) connected to a remote network (10.10.10.0/24) via a router.<br>
•	Devices include PCs, switches, hub, and wireless AP.<br>
(Insert screenshot of your Packet Tracer setup here)<br>
<img width="823" height="695" alt="image" src="https://github.com/user-attachments/assets/d5254b5a-4ad7-404e-949e-f9bab01e241e" />

________________________________________
# IP Addressing Table
(Example – actual values from simulation)<br>
Device	IPv4 Address	Subnet Mask	MAC Address<br>
PC-A	172.16.31.5	255.255.255.0	00D0:D311:C788<br>
PC-B	172.16.31.2	255.255.255.0	000C:85CC:1DA7<br>
Router (G0/0)	172.16.31.1	255.255.255.0	00D0:BA8E:741A<br>
PC-Remote	10.10.10.2	255.255.255.0	00D0:588C:2401<br>
________________________________________
# Procedure
# Part 1: Local Network Communication
1.	Click PC-A (172.16.31.5) and open the Command Prompt.<br>
2.	Enter ping 172.16.31.2.<br>
3.	Switch to Simulation Mode and repeat the ping.<br>
4.	When the PDU appears, click it and record: Destination MAC, Source MAC, Source IP, Destination IP, and the device name.<br>
5.	Use Capture/Forward to follow the PDU through the network until it reaches PC-B.<br>
6.	Record the information in a table.<br>
7.	Repeat the above process for:<br>
o	Ping from 172.16.31.3 to 172.16.31.2<br>
o	Ping from 172.16.31.5 to 172.16.31.4<br>
Part 2: Remote Network Communication<br>
1.	From PC-A (172.16.31.5), enter ping 10.10.10.2.<br>
2.	Switch to Simulation Mode and repeat the ping.<br>
3.	When the PDU appears, note the Destination MAC, Source MAC, Source IP, and Destination IP.<br>
4.	Follow the PDU step-by-step until it reaches the remote PC.<br>
5.	Observe how MAC addresses change at the router while IP addresses remain constant end-to-end.<br>
________________________________________
# Example Data Recording Table
At Device	Dest. MAC	Src MAC	Src IPv4	Dest IPv4<br>
172.16.31.5	000C:85CC:1DA7	00D0:D311:C788	172.16.31.5	172.16.31.2<br>
Switch1	000C:85CC:1DA7	00D0:D311:C788	N/A	N/A<br>
172.16.31.2	00D0:D311:C788	000C:85CC:1DA7	172.16.31.2	172.16.31.5<br>
________________________________________
# Output (Screenshots)
•	PDU details for local communication<br>
<img width="1560" height="698" alt="Screenshot 2026-11-17 172134" src="https://github.com/user-attachments/assets/b1b04c56-048e-4422-b23a-033877c75581" />
<img width="1537" height="785" alt="Screenshot 2026-11-17 173046" src="https://github.com/user-attachments/assets/17f229d7-b269-4511-9155-46d35e943498" />
<img width="1567" height="787" alt="Screenshot 2026-11-17 173213" src="https://github.com/user-attachments/assets/b9b25cec-3fc4-4588-af63-8df7ca5b7ece" />



•	PDU details for remote communication<br>
<img width="1538" height="796" alt="Screenshot 2026-11-17 174542" src="https://github.com/user-attachments/assets/bfd4371a-26d0-43da-8d63-702756d5a0da" />
<img width="1512" height="697" alt="Screenshot 2026-11-17 173912" src="https://github.com/user-attachments/assets/a7b908e7-6fe9-47cc-9f56-89fc8d777c70" />


•	Tables showing MAC/IP changes through each device<br>
<img width="727" height="358" alt="Screenshot 2026-11-17 173309" src="https://github.com/user-attachments/assets/fa19719e-c0f5-4347-a8d6-50f8198331cb" />

<img width="707" height="278" alt="Screenshot 2026-11-17 173810" src="https://github.com/user-attachments/assets/c69519ed-7f3c-4221-906e-be85b2d3f0c5" />


________________________________________
# Result
Successfully captured and analyzed MAC and IP addresses for both local and remote communications. Verified that MAC addresses change at each hop while IP addresses remain constant from source to destination.


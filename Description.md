# Small Manufacturing Company
Configuring VLANs, ROAS, OSPF, DHCP, SSH & Port Security for a small manufacturing company using Packet Tracer

![small-mfg-comp](https://github.com/faliqfizi/small_mfg_comp/assets/140976235/e455331d-fc96-4a1f-b85d-c1d9e8cb943c)

### 1.	Assigning IP Addresses:
#### a.	to each department with correct subnets
#### b.	to each router’s network interfaces

1st Floor:

  •	IT- VLAN 10: 192.168.1.0 /24
  
  • Admin – VLAN 20: 192.168.2.0 /24


2nd Floor:

  •	Sales- VLAN 30: 192.168.3.0 /24
  
  •	HR- VLAN 40: 192.168.4.0 /24
  
  •	Finance- VLAN 50: 192.168.5.0 /24


3rd Floor:

  •	Quality- VLAN 60: 192.168.6.0 /24
  
  •	Maintenance- VLAN 70: 192.168.7.0 /24
  
  •	Production- VLAN 80: 192.168.8.0 /24

#### Routers:
  • R-F1 and R-F2: 10.10.10.8 /30
  
  • R-F1 and R-F3: 10.10.10.4 /30
  
  • R-F2 and R-F3: 10.10.10.0 /30

### 2.	Configure VLANs
-	Assign each department to different VLANS
-	Configure static access mode to the switchports that are connected to end hosts
-	Configure trunk mode to the switchports that are connected to the router

### 3.	Configure Router on a stick (ROAS)
-	Create sub interfaces on the routers with encapsulation type of dot1q
-	Assign IP addresses for each sub interfaces with a correct subnet 

### 4.	Configure OSPF as the dynamic routing protocol
-	Configure OSPF for each router serial connection
-	For serial connections, configure the clock rate to 64000 Kbps
-	Configure OSPF for each router sub interfaces

### 5.	Configure DHCP
-	Enable DHCP service on each router (to configure the routers as DHCP servers)
-	Create a DHCP pool & network for each department
-	Configure each router as the default gateway and the DNS server
-	Access to each PCs to obtain their IP addresses with DHCP

### 6.	Configure SSH
-	Configure SSH on all router’s VTY line
-	Assign the PC on IT department as Test-PC to use it for remote login.

### 7.	Configure Port Security
-	Configure port-security to IT dept switch to only allow Test-PC to access port f0/2
-	Violation mode: shutdown
-	Mac address: sticky


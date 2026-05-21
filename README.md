# 🏥 Hospital Network System
### Implementation Using Cisco Packet Tracer

> A simulated hospital network built with two routers and six VLANs for different hospital departments — designed as part of Computer Networks at University of Narowal.

---

## 👥 Team Members

| Name | Roll No |
|------|---------|
| Muhammad Talha | 23-uon-0446 |
| Nahah Butt | 23-uon-0338 |
 
**Subject:** CS-205 — Computer Networks  
**Degree:** BS Computer Science  
**University:** University of Narowal

---

## 🗺️ Network Overview

The hospital network is divided into **6 VLANs**, each representing a department:

| VLAN | Department | Subnet | Gateway |
|------|------------|--------|---------|
| VLAN 10 | Administration | 192.168.2.0/24 | 192.168.2.1 |
| VLAN 20 | Reception | 192.168.2.0/24 | 192.168.2.1 |
| VLAN 30 | Doctors & Nurses | 192.168.2.0/24 | 192.168.2.1 |
| VLAN 40 | Patients Ward | 192.168.3.0/24 | 192.168.3.1 |
| VLAN 50 | Pharmacy | 192.168.3.0/24 | 192.168.3.1 |
| VLAN 60 | Laboratory | 192.168.3.0/24 | 192.168.3.1 |

Two routers handle inter-network routing between the two sides of the hospital network.

---

## ⚙️ How to Open the Simulation

1. Download **Cisco Packet Tracer** for free from [Cisco Networking Academy](https://www.netacad.com/courses/packet-tracer)
2. Create a free account and log in
3. Clone or download this repository
4. Open `hospital_network.pkt` in Packet Tracer
5. Click any device to inspect its configuration

---

## 🔧 Key Configurations

**Router interfaces** were configured with static IP addresses and activated using `no shutdown`.

**Switch VLANs** were created and ports assigned in access mode. Trunk links connect switches to routers.

**Routing** was configured statically to allow communication between both sides of the network.

To verify connectivity inside Packet Tracer:
```
PC> ping 192.168.3.1       # ping across routers
Router# show ip route      # check routing table
Switch# show vlan          # check VLAN assignments
```

---

## 📚 Concepts Covered

- IP Addressing & Subnetting
- VLAN Configuration & Trunking
- Inter-VLAN Routing
- Static Routing
- Network Troubleshooting (ping, traceroute)

---

## 📄 License

This project was created for academic purposes at the University of Narowal. Feel free to use it as a reference for learning.

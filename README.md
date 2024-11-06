## Network Security

### Raspberry Pi Wireless Access Point (AP)

***Author: Jainil Vakharia***

#### 1. Project Overview

The project implements a secure network access point using a Raspberry Pi, configured with firewall functionality and a VPN, and equipped with Adblock for enhanced privacy and security. This setup provides a controlled network environment where connected devices are shielded from unwanted or harmful traffic through ad filtering and firewall rules. The goal is to create a versatile access point capable of managing both local and remote network traffic securely.


#### 2. Project Goals

The primary objectives of the project include:

- Establish a Portable Secure Router: Configure a Raspberry Pi as a Wi-Fi router with a VPN to ensure encrypted connectivity and protect data privacy.

- Implement Adblock as a Firewall Solution: Use Adblock for traffic filtering, enhancing security by blocking ads and potentially malicious content before they reach client devices.

- Create a Secure Network Access Point: Facilitate safe, reliable connectivity for multiple devices over a single, secure access point that protects users’ data from external threats.

#### 3. Components Used

- Raspberry Pi 4B
- OpenWRT Firmware
- Network Interface Card (NIC) (Optional)

#### 4. Project Implementation

##### 4.1 Router Configuration

**OpenWRT Installation:**
Install OpenWRT firmware on the Raspberry Pi 4B to transform it into a functional router. OpenWRT’s interface allows configuration of routing protocols, firewall, and network interfaces.

**Routing Setup:**
Configure static and dynamic routing protocols as required for both local and VPN-based traffic. Define network interfaces to manage different types of traffic, including Local Area Network (LAN), Wireless Local Area Network (WLAN), and VPN connections.

  

##### 4.2 Firewall and Adblock Configuration

**Adblock Installation:**
Install and configure the Adblock package available through OpenWRT to filter out ads and malicious content from network traffic. Adblock functions as a preventive security layer, filtering out network requests to ad servers and known malicious domains.

**Firewall Rule Definition:**
Configure firewall rules within OpenWRT to enforce security policies, leveraging IP filtering, port management, and stateful packet inspection. Define rule sets for both inbound and outbound traffic:

**IP Filtering:** Restricts access based on IP addresses to prevent unauthorized access.
**Port Management:** Limits access to specific network ports, allowing only essential services.
**Stateful Inspection:** Monitors packet state and sequence to allow only secure, legitimate traffic.

**VPN Configuration:**
Install a VPN client on the Raspberry Pi to create a secure, encrypted tunnel for data transmission. Configure the VPN client to route all connected device traffic through the encrypted connection, masking IP addresses and ensuring data privacy.
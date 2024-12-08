
# VPN Setup and Usage with ProtonVPN

In this home lab, I will practice creating an Azure Virtual Machine (VM) and downloading a VPN client from within that VM. I will document the different IP addresses and experiment with websites when the VPN is connected to a server in another country.

## Environments and Technologies Used:
- **Microsoft Azure** (Virtual Machines/Compute)
- **Remote Desktop**
- **Proton VPN**

## Operating System:
- **Windows 10** (21H2)

## Steps:

### 1. Create Virtual Machine in Azure:
- Browse to [WhatIsMyIPAddress](https://whatismyipaddress.com/) **from your own machine** and take note of your IP address in a text file.
- Create a **Resource Group** in Azure.
- Create a **Windows 10 Virtual Machine** in another geographic location (try a different country).
  - Log into the VM using **Remote Desktop**.
  - Browse to [WhatIsMyIPAddress](https://whatismyipaddress.com/) within the VM and note the IP address in a text file.

![image](https://github.com/user-attachments/assets/dd30f6a1-bc59-4562-8b3e-b016beaaa9d5)

### 2. Sign up for ProtonVPN and test the VPN connection:
- On your actual computer, sign up for the free version of Proton VPN at [ProtonVPN Signup](https://account.protonvpn.com/signup?plan=free&language=en).
- Within your VM, download the **Proton VPN client**.
  - Log in to ProtonVPN at [ProtonVPN Login](https://account.protonvpn.com/login) and choose a VPN server in a different country (e.g., Japan).
  - Browse to [WhatIsMyIPAddress](https://whatismyipaddress.com/) and note the new IP address.
- Test browsing websites like **Google**, **Disney**, and/or **Amazon** to see if there are any differences based on the VPN's server location. For example, you may notice changes in the language or URL.

![image](https://github.com/user-attachments/assets/77b0905f-116c-4126-a656-214df4903240)

---

### IP Address Examples:

**VM (Non-VPN)**  
- IPv4: `172.214.244.206`  
- ISP: Microsoft Limited  
- City: Chicago  
- Region: Illinois  
- Country: United States

**VM (With VPN)**  
- IPv4: `212.8.250.219`  
- ISP: WorldStream B.V.  
- Services: Network Sharing Device  
- City: Bucharest  
- Region: Bucharest  
- Country: Romania

## Key Takeaways:

- **Azure Virtual Machines (VMs):** Demonstrates creating and managing VMs in Microsoft Azure and accessing them via Remote Desktop.
  
- **IP Geolocation:** Shows how the IP address changes based on the geographic location of the VM, emphasizing the impact of IP addresses on location-based services.

- **VPN Functionality:** Illustrates how ProtonVPN masks the real IP address, allowing you to appear as if browsing from another country, enhancing privacy.

- **Geolocation Testing:** Observes how websites like Google, Amazon, and Disney change content (language, currency, etc.) based on VPN server location.

- **Security and Privacy:** Highlights the role of VPNs in securing browsing and protecting privacy by encrypting traffic and masking the real IP.

- **Hands-On Experience:** Provides practical experience with setting up VMs and VPNs, valuable for cloud computing, networking, and cybersecurity fields.

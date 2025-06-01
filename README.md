# Active Directory Deployment Using Powershell Automation
## Objective
In this lab we're going to walk through how to create an Active Directory home lab Environment using Oracle Virtual Box and automating AD deployments using Powershell. Configuring and running this lab will definitely help develop your understarding of how active directory and windows networking works, so I'd highly recomend running through it a couple tines, ask questions where stuff is unclear, and eventually try to butld it on your own. Please let me know 1f you have any questions!

### 🔧 Tools & Technologies Used:
- Oracle VirtualBox
- VMware
- Windows Server 2019 ISO
- Windows 10 ISO
- PowerShell
- DHCP / NAT / Routing
- Active Directory (AD DS)
  
## Skills Practiced:

- Network configuration (NAT, DHCP, static IPs)
- Active Directory deployment & domain management
- PowerShell scripting for bulk operations
- Cross-platform virtualization (VirtualBox + VMware)
- Troubleshooting client-server domain connectivity

## Setup & Configuration Process:

### Environment Preparation:
- Installed VirtualBox and VMware Workstation.
- Downloaded and mounted Windows Server 2019 and Windows 10 ISOs.
 
 *Ref 1: Mounting Windows Server 2019 in Oracle Virtual Box* [![Capture.png](https://i.postimg.cc/wTbSqCb3/Capture.png)](https://postimg.cc/HVXS3hmC)
### Server Installation:
- Installed Windows Server 2019 on VirtualBox.
- Configured the server with a static IP address within the internal network.
- Enabled NAT/Routing for external connectivity.
 
*Ref 2: Launching Windows Server 2019 in Oracle Virtual Box* [![Capture.png](https://i.postimg.cc/jScnnhPW/Capture.png)](https://postimg.cc/VJSk3n71)
### Active Directory & Domain Configuration:
- Installed Active Directory Domain Services (AD DS).
- Promoted the server to a Domain Controller.
- Created a custom domain name for the lab environment.

*Ref 3: Installing Active Directory Software* [![Capture.png](https://i.postimg.cc/hvNbw1p4/Capture.png)](https://postimg.cc/SY7MY8BH)
### DHCP Setup:
- Installed and configured DHCP Server role on Server 2019.
- Set up an internal DHCP scope to automatically assign IPs to client machines.
- Ensured DHCP does not conflict with the home router’s IP range.

*Ref 4: Setting up DHCP* [![Capture.png](https://i.postimg.cc/HLtzx5s3/Capture.png)](https://postimg.cc/HJVXvrM7)
### PowerShell Automation:
- Wrote and executed a PowerShell script to automatically create 1,000+ user accounts in Active Directory.
- Verified accounts using Active Directory Users and Computers (ADUC).

*Ref 5: Automated the Creation of 1,000+ user accounts using PowerShell Script* [![Capture.png](https://i.postimg.cc/2ydhcNbG/Capture.png)](https://postimg.cc/gLJxj5KL)
### Client Machine Integration:
- Created a Windows 10 client VM in VMware.
- Joined the client VM to the domain using credentials from the bulk-created AD user accounts.
- Tested login with multiple users to ensure successful domain authentication.

*Ref 6: Joining the Client VM to the Domain [![Capture.png](https://i.postimg.cc/MT2nhr8F/Capture.png)](https://postimg.cc/2qGjWGyQ)*

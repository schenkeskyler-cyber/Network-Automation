# Network Device Automation using Ansible

## Module Information
- **Module:** Network Programmability  
- **Module Code:** ACCB5029  
- **Assessment:** Implementation as a Group and Demonstration  

---

## Team Members and Roles
Rehan Joseph – Network Engineer
Responsible for designing the network topology, configuring physical routers and switches, and verifying baseline settings.

Skyler Schenke – Automation Engineer
Developed Ansible playbooks and inventory files, ensuring automation tasks worked correctly on physical devices.

Leo Richards – DevOps & Documentation Lead
Managed the GitHub repository, version control, testing, documentation, and assisted with troubleshooting.


Although roles were defined, all team members collaborated throughout the project and supported each other where required.

---

## Project Overview
This project demonstrates the automation of network device configuration using **Ansible**.  
The aim is to reduce manual configuration effort, minimise human error, and apply Infrastructure as Code principles to network management.

A virtual Cisco router was used to design, implement, and test the automation solution in a controlled environment suitable for demonstration.

---

## Technologies and Tools Used
- Ansible  
- Cisco IOS 
- SSH  
- GitHub (Version Control and Collaboration)  
- Discord (Team Communication)

Additional tools and features may be integrated as part of extended research and implementation.

---

## Automation Scope
The automation scope was deliberately kept focused to ensure reliability and clarity during demonstration.  
The following configurations are automated:
- Hostname configuration  
- IP addressing  
- SSH configuration  

---

## Repository Structure
Physical devices were configured for SSH access to allow Ansible to connect securely. The management PC ran Ansible, using an inventory file containing all device IPs.

We developed a series of Ansible playbooks:

Main playbooks: One for all router configurations, one for all switch configurations

Additional smaller playbooks: Task-specific updates as needed

Router playbooks configured IPs, routing, and static routes; switch playbooks handled VLANs, port assignments, and port security. All configurations were applied via Cisco-specific Ansible modules. Verification was done using IOS commands (show run, show ip interface brief, show ip route) to ensure accuracy and consistency.

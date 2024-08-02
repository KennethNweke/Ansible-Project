# Ansible-Project
I used Ansible to streamline  network management tasks by creating a router group and pulling configuration information

## Objective
In this project, I utilized Ansible, a powerful IT automation tool, to manage and interact with a Cisco 1900 router within a network. The network configuration for this setup included an IP address of 192.168.56.107/24. My tasks encompassed installation, configuration, and execution of various Ansible modules to ensure seamless communication and configuration management of the router.

## Key Tasks and Achievements
### Installation and Setup:
- Installed Ansible on an Ubuntu system to serve as the automation controller.
- Configured the Ansible environment, including modifications to the ansible.cfg file and the hosts inventory file to enable SSH connectivity and handle SSH fingerprinting appropriately.

### Setup Used 
![image](https://github.com/user-attachments/assets/847b366d-2123-4f09-ab20-4da5512fc852)

### Router Group Creation:
- Defined a group for the router in the Ansible hosts file, identifying it as a member of the ciscoRouters group.
- Configuration entry example in hosts file:
  - [ciscoRouters] 192.168.56.107
 
### Router Configuration:
- Set up SSH on the Cisco 1900 router and configured its interface with the IP address to enable communication with the Ansible controller.

### Connectivity Verification:
- Conducted a series of pings to the router to verify network connectivity and performance using Ansible's ping module.
- Command executed
  - ansible ciscoRouters -m ping
- This confirmed that the router was reachable and the network was reliable.

### Configuration Management:
- Pulled network configuration parameters from the router using Ansible's ios_command module.
- Command executed:
  - ansible ciscoRouters -m ios_command -a "commands='show ip interface brief'"
- This command retrieved and displayed the IP interface brief, providing crucial information about the router's interface configurations.

### Skills and Tools Utilized
- Tools: Ansible, Cisco IOS, Ubuntu
- Skills: Network Automation, Ansible Playbooks, SSH Configuration, Network Troubleshooting
- Commands: Ansible modules such as ping and ios_command
- Configuration Files: Ansible hosts inventory, ansible.cfg



## Watch the video on YouTube or [View on LinkedIn](https://www.linkedin.com/posts/kenneth-nweke-4a9456185_networkautomation-ansible-cisco-activity-7223960575465168896-3jzL?utm_source=share&utm_medium=member_desktop)
[![Link to YouTube Video](https://img.youtube.com/vi/q0DuZ_mXMuQ/0.jpg)](https://youtu.be/q0DuZ_mXMuQ)



### Outcome
The successful implementation of Ansible for network automation on a Cisco 1900 router showcased the potential for efficient network management and configuration retrieval. This project highlighted my ability to set up and configure automation tools, troubleshoot network connectivity, and manage network devices programmatically.


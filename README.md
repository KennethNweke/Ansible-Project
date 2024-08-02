# Ansible-Project
I used Ansible to streamline  network management tasks by creating a router group and pulling configuration information

## Objective
In this project, I utilized Ansible, a powerful IT automation tool, to manage and interact with a Cisco 1900 router within a network. The network configuration for this setup included an IP address of 192.168.56.107/24. My tasks encompassed installation, configuration, and execution of various Ansible modules to ensure seamless communication and configuration management of the router.

## Key Tasks and Achievements
### Installation and Setup:
- Installed Ansible on an Ubuntu system to serve as the automation controller.
- Configured the Ansible environment, including modifications to the ansible.cfg file and the hosts inventory file to enable SSH connectivity and handle SSH fingerprinting appropriately.

### Router Group Creation:
- Defined a group for the router in the Ansible hosts file, identifying it as a member of the ciscoRouters group.
- Configuration entry example in hosts file:
  - [ciscoRouters] 192.168.56.107
 

### Router Configuration:

- Set up SSH on the Cisco 1900 router and configured its interface with the IP address to enable communication with the Ansible controller.

### Connectivity Verification:
Conducted a series of pings to the router to verify network connectivity and performance using Ansible's ping module.
Command executed

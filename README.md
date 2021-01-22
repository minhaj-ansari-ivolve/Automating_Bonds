# Automating Bonds

## Introduction

It will automate the process of creating Bonds and Bridges on CentOS 8.3. It will also automate the process of installing KVM and installing another CentOS above the KVM using Vittual Machine Manager. The whole automation is done by Ansible.

## Modules being Automated

1. Configure Slave Interfaces
2. Configure Channel Bonding Interface
3. Create VLAN Interface
4. Create Bridge
5. Installing KVM
6. Hosting CentOS 8 Kickstart file on NGINX
7. Creating VM on KVM with CentOS 8 installed

## Notes

- Ansible should be installed to use this automation
- Change the host file of Ansible according to the ip of your machine.
- Internet Connectivity is necessary to install dependencies while the automation is running. 

## CLI Commands

```
ansible-playbook -i hosts -K Automation.yml
```

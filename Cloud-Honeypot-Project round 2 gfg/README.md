# Cloud-Honeypot-Project (Vultr)

## Objective

The Cloud honeypot lab aims to create a practical and portable honeypot environment to analyze and observe incoming cyber attacks from around the world. This honeypot implementation focuses on setting up a duplicate environment for attackers to target in a possible enterprise network, completely in the cloud where it is safe from any possible host machine infection. This exercise helps build an understanding of how a honeypot works and how to ingest logs and data collected to recognize patterns and to possibly throw off attackers from hitting the main network. 

### Skills Learned

- Cloud Virtual Machine Implementation
- Firewall and port configuration to block unwanted inbound traffic (Cloud)
- Tpot honeypot setup and installation 
- Attack map and Kibana dashboard setup to ingest honeypot log data and analysis

### Tools Used

- Vultr Cloud Platform
- Debian Live Image
- Tpot Honeypot (Attack map + Kibana Dashboard)

## Steps

#### 1. Setup Cloud VM with Vultr using Tpot
- Created Vultr account and started a new instance with Debian 12
- Configured the Virtual Machine’s firewall settings to block outside internet connections from interacting with honeypot (for now).


#### 2. Setting Up Tpot
- Started initial setup of Debian (CLI)
- Logged in as root and created a new user and added them to sudoers file to installed Tpot  properly using script
- Ran the installation script and created new username and password for the Tpot web application/interface
- Logged into the web interface using IP address (cloud) with port and specifying user and password
- Successfully logged into Tpot web user interface 

![1]
![2]

#### 3. Using Tpot Attackmap & Kibana

- Started to reconfigure the firewall to start receiving incoming connections to the specified port of the Tpot web interface
- From the web interface I've selected Attackmap and viewed the incoming connections from honeypot
- Opened kibana honeytrap dashboard and viewed data
- Ran honeypot for a significant amount of time to have data generated to Kibana dashboard and prepared for future analysis
![3]
![4]

[1]: https://github.com/NODRYC/Cloud-Honeypot-Project/blob/main/pics/tpot-installed.png
[2]: https://github.com/NODRYC/Cloud-Honeypot-Project/blob/main/pics/tpot-logon.png
[3]: https://github.com/NODRYC/Cloud-Honeypot-Project/blob/main/pics/tpot-attack-map.png
[4]: https://github.com/NODRYC/Cloud-Honeypot-Project/blob/main/pics/kibana-dashboard.png

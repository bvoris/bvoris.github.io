---
layout: post
title: Ransomware and my experience
categories: [content, Ransomware]
---
# Ransomeware
I've been engageed with the community for some time now. One of the greatest blights facing technologists today is Ransomware. 

What is ransomware?
"Ransomware is a type of malware from cryptovirology that threatens to publish the victim's personal data or perpetually block access to it unless a ransom is paid. While some simple ransomware may lock the system without damaging any files, more advanced malware uses a technique called cryptoviral extortion." - Wikipedia

Ransomware has been around since the mid to late 90s but really didn't start becoming a serious problem until the mid to late 2010s. Threat actor and hacker groups use a combination of tools and social engineering to gain access to a network and its sensitive data. Usually data is exfiltrated from the network as a copy and then a crypto-locking software infects all the files and systems on the victim network.

# So what have I personally seen and dealt with?
Outside of your run of the mill hackathons, virus infections, malware deployments, skimming etc. I've run into 3 catastrophic ransomware infections. I'll provide some detail (not the organizations name, or industry) and my role for that particular incident.

1) Small business of less than 10 employees with a small office network infected with ransomware which took out their VMs, all of their files and exfiltrated client/payment lists. My role for this incident was as a consultant assisting their MSP consultants with review, remediation and recovery. I was able to work remotely with the MSP consultants to shutdown, clean up, patch all systems on the network. The organizations VMs were encrypted which had their data, they did have a local back up of their data which was plugged in at the time and encrypted as well. They had offline backups which were outdated and not verified. I was able to use some data recovery tools and recover the VM files. From there I was able to mount the volumes and recover the data. The VMs were rebuilt and their current data was subsequently uploaded to the new servers. The ransom was not paid for this incident and what ever the threat actors were able to get, they ultimately had.

2) 

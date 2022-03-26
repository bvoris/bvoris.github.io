---
layout: post
title: Ransomware and my experience
categories: [content, Ransomware]
---
# Ransomware
I've been engageed with the community for some time now. One of the greatest blights facing technologists today is Ransomware. 

What is ransomware?
"Ransomware is a type of malware from cryptovirology that threatens to publish the victim's personal data or perpetually block access to it unless a ransom is paid. While some simple ransomware may lock the system without damaging any files, more advanced malware uses a technique called cryptoviral extortion." - Wikipedia

Ransomware has been around since the mid to late 90s but really didn't start becoming a serious problem until the mid to late 2010s. Threat actor and hacker groups use a combination of tools and social engineering to gain access to a network and its sensitive data. Usually data is exfiltrated from the network as a copy and then a crypto-locking software infects all the files and systems on the victim network.

# So what have I personally seen and dealt with?
Outside of your run of the mill hackathons, virus infections, malware deployments, skimming etc. I've run into 3 catastrophic ransomware infections. I'll provide some detail (not the organizations name, or industry) and my role for that particular incident.

1) Small business of less than 10 employees with a small office network infected with ransomware which took out their VMs, all of their files and exfiltrated client/payment lists. My role for this incident was as a consultant assisting their MSP consultants with review, remediation and recovery. I was able to work remotely with the MSP consultants to shutdown, clean up, patch all systems on the network. The organizations VMs were encrypted which had their data, they did have a local back up of their data which was plugged in at the time and encrypted as well. They had offline backups which were outdated and not verified. I was able to use some data recovery tools and recover the VM files. From there I was able to mount the volumes and recover the data. The VMs were rebuilt and their current data was subsequently uploaded to the new servers. The ransom was not paid for this incident and what ever the threat actors were able to get, they ultimately had.

2) Med to large buisness with offices across the US suffered a similar incident. Their entire network was taken down due to poorly managed infrastructure that allowed threat actors to remotely access the network, monitor the network and systems. Eventually the threat actors deployed ransomware which encrypted all systems, and backups. My role was as an outside consultant to recommend infrastructure and security best practices while helping them maintain a level of sanity. This was a very short stint and they were able to rebuild the majority of their systems and recover some but not all of their data without paying the ransom.

3) Large global organization with a failed ransomware deployment into their corporate headquarters. The network, firewall and remote capabilities were completely taken offline for several days. While the ransomware deployment was unsuccessful the organization suffered a breach, which lead to a lost of IP and sensitive data. This incident was caused by an unpatched firewall, being publically exposed. Threat actors ran a script on the firewall, gained access to all of the provisioned accounts on the firewall which were also local network administrator and active directory administrator accounts. This allowed the threat actors to have unteathered access to the network, exfiltrate data and attempt to deploy ransomware. Luckily a newly introduced endpoint protection solution prevented the infections, and alerted the technology department to the incident. They shutdown their network, systems, brought in multiple consultants to review and verify. The only thing they wanted proof on was how the threat actors gained access to the network. They assumed the firewall and took it offline. I was called in and asked to replicate the attack based on the minimal information I had about the firewall and network. I was given an IP address to the firewall which was now sandboxed, and was able to run a Proof of Concept exploit which took less than 10 minutes. I extracted all usernames and passwords from the firewall. I provided a write-up, and was done.

# Conclusion
While these incidents were catastrophic for the organizations and caused significant downtime which resulted in a loss of profits ALL of them could have been avoided.
Proper security hygiene of logging, monitoring, patching and replacement of EoL legacy machines could have saved these orgs from this loss.

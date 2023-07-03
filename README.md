## Lab Setup: Analyzing failed Brute force RDP Attacks on Honeypot VM and Analyzing the logs using SIEM
### [Step-by-step tutorial article](https://medium.com/@okeyopaul/creating-a-honeypot-windows-10-virtual-machine-and-analyzing-the-logs-using-microsoft-sentinel-985b57979c41#5258)
<img src="https://github.com/paulokeyo/failedRDPAttacks/blob/main/assets/Azure%20resources.png?raw=true"/>
A Windows 10 VM was setup and acted as our public facing VM to the internet. Log Analytics workspace was used to collect Windows Security events from the VM. A custom alert rule was created in Microsoft Sentinel SIEM which analyzed the logs for the VM in the Log Analytics workspace  
<img src="https://github.com/paulokeyo/failedRDPAttacks/blob/main/assets/SIEM%20alert%20rule.jpg?raw=true"/>
The alert rule is set to alert every 1hr incase an incident has occurred in the past one hour

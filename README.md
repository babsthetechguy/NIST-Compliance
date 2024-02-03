# Implementing Security Controls Towards NIST SP 800-53 R5 Compliance![Screenshot (351)](https://github.com/babsthetechguy/NIST-Compliance/assets/150613649/b99aa6c2-cca9-43cf-be84-6c15bf22bdf2)



# Introduction
In this project, I remediate my mini honeynet I created in the previous project [(Building a SOC + Honenet)](https://github.com/babsthetechguy/Cyber-Course) to be up to par and compliant with NIST SP 800 53 R5 regulatory compliance standards. I resolved several non-compliant controls within the security metrics in Microsoft Azure to harden the environment and decrease/nullify attacks as well as keeping the environment up to compliant standards.  The compliance metrics we will mitigate and audit are:

- AC: Access Control
- AU: Audit and Accountability 
- CP: Contingency Planning
- IA: Identification and Authentication
- IR: Incident Response
- RA: Risk Assessment
- SC: System and Communications Protection
- SI: System and Information Integrity


## Ratings Before Hardening/Security Controls

![Screenshot (352)](https://github.com/babsthetechguy/NIST-Compliance/assets/150613649/bcbdf3ad-6672-475f-83a6-1e0b3534ed90)

![Screenshot (353)](https://github.com/babsthetechguy/NIST-Compliance/assets/150613649/f431744a-89d4-4ee6-b1fc-dd14c95d313c)




## Metrics Before Hardening /Security Controls

Some of the more common compliance issues were the lack of encryption & having email notifications for security alerts. as well as Microsoft Defender configuration/

![Screenshot (353)](https://github.com/babsthetechguy/NIST-Compliance/assets/150613649/8b16a38c-0891-4cca-ac40-45a5ec545b1c)



In addition to regular compliance issues there were “Quick Fixes”, such as Microsoft defender being enabled for different sources to match approved compliant status, with a HIGH severity. <br/>

![Screenshot (354)](https://github.com/babsthetechguy/NIST-Compliance/assets/150613649/60ab809f-909a-488c-be1f-c4e4dc89fb7d)



Each compliance tool had different freshness intervals as well from the lower end 30 minutes to 24 hours to verify compliance approval. 


# IMPLEMENTATION:

We started with the AC: Access control compliance controls with AC: 2 and ended with putting the SC: System and Communications Protection to compliance. Throughout I implemented both the Manual option options as well as Quick Fix & exemption tools when applicable.  


![Screenshot (355)](https://github.com/babsthetechguy/NIST-Compliance/assets/150613649/8a30eb21-cb65-4b9f-98c6-a446c5878b37)


![Screenshot (347)](https://github.com/babsthetechguy/NIST-Compliance/assets/150613649/97196489-8c8b-49cb-8309-36d3e23c58f2)




⭐ <b>Some Of The Common Remediation Functions To Fix:</b> 
- Firewall Creations for VMs (linux/Windows)
- Email Notifications
- Exemptions
- Enabling of Microsoft defender for resource manager, DNS, etc. 
- Azure Backup for virtual machines
- Purge Protection
- Subnets associated with network security groups <br/>


⭐ <b>Some Of The Common Techniques (categories) Fixed during remediation.</b>
- Defense Evasion (https://attack.mitre.org/tactics/TA0005/)
- Privilege Escalation (https://attack.mitre.org/tactics/TA0004/)
- Impact (https://attack.mitre.org/tactics/TA0040/)
- Persistence (https://attack.mitre.org/tactics/TA0003/)
- Exfiltration (https://attack.mitre.org/tactics/TA0011/)
- Lateral Movement (https://attack.mitre.org/tactics/TA0008/)




## Ratings AFTER Hardening/ Security Controls

The metrics shown below is after 24 hours of our last policy edit, showing increase in not only the NIST framework but also in the Microsoft Cloud security Benchmark controls as well. 


![Screenshot (348)](https://github.com/babsthetechguy/NIST-Compliance/assets/150613649/eb2d78c2-b5bb-40b2-8ac9-e4b250dab26d)



## Metrics AFTER Hardening/ Security Controls

As shown below majority of all compliance policies were mitigated


![Screenshot (349)](https://github.com/babsthetechguy/NIST-Compliance/assets/150613649/a10c0004-6c1a-48e6-a60c-cfcb22344c90)



# Conclusion

In this project, NIST SP 800 53 R5 policy changes were made within the Azure environment to become more compliant with regulations. Utilizing the tools available we were able to create firewalls for our virtual machines, create backups for virtual machines, create subnets with our NSGS, enable Microsoft Defender for several resources and more. It is noteworthy that the number of security events and incidents were drastically reduced after the security controls were applied, demonstrating their effectiveness [as shown in previous Azure SOC + Honeynet lab](https://github.com/babsthetechguy/Cyber-Course)

It is worth noting that remediating the environment to be more compliant with NIST SP 800 53 5 also increased our compliance with the Microsoft Cloud Security Benchmark (Azure default), increasing our overall score to a whopping <b>88%</b> Secure Score!


![Screenshot (350)](https://github.com/babsthetechguy/NIST-Compliance/assets/150613649/37c3c3b4-187d-46b8-9337-8fac7390d6fa)






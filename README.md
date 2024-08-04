***DISCLAIMER:*** *This is intended for ethical hacking educational purpose. Performing hacking attempts on any computers that you do not own (without permission) is illegal! Do not attempt to gain access to devices that you do not own!*

# <div align="center"> Harvesting Credentials</div>

## Introduction

In todays digital landscape, the threat of cyber-attacks, particularly through phishing, has become a signigicant concern for individuals and organizations alike. Phishing attacks, which often involve tricking individuals into revealing sensiitive information such as login credentaisl, continue to be a prevalant method emplyed by cybercriminals. 

This project delves into a specific instance of phishing simulation, showacsing teh user of sophisticated tools and techniques to harvest credentials. It aims to provide an in-depth analysis of a phishing scenario, where a LinkedIn-themed phishing attack was deployed to engage a target through professional networking channel. The choice of LinkedIn as the phishing template was strategic, given the platforms credibility and the likelihood of successful interaction by the target. 

***Architecture of Harvesting Credentials***

- ***Kali Linux*** - linux distribution designed for digital forensics and penetration testing
- ***Zphisher*** - a powerful open-source Phishing tool
- ***The Socail-Engineer Toolkit (SET)*** - an open-source penetration testing framework designed for social engineering.


## Choice of a Web Template

The LinkedIn template is chosen for its relevance to the pretexting scenario, which involves engaging with Dr. Alexander through professioanl networking. LinkedIn is a trusted platform for professionals and using this template in the phishing attack increases the likelihood of Dr. Alexander interacting with it.

## Step-by-Step Deployment

***Step 1: Zphisher installation for Linux***
<p align="center"><img src=images/Picture1.png></p>
<p align="center"><img src=images/Picture2.png></p>

---

***Step 2: Zphisher setup for LinkedIn Phishing page***
<div align="center">Select option [14] LinkedIn</div>
<p align="center"><img src=images/Picture3.png></p>
<div align="center">Select option [2] Cloudflard a port forwarding service</div>
<p align="center"><img src=images/Picture4.png></p>
<div align="center">Select option N for do you want a custom port</div>
<p align="center"><img src=images/Picture5.png></p>
<div align="center">Copy URL 1 Link to use in SET to send the email</div>
<p align="center"><img src=images/Picture6.png></p>

---

***Step 3: The Social-Engineer ToolKit (SET) setup to craft and send the phishing email***
<div align="center">Run SET</div>
<p align="center"><img src=images/Picture7.png></p>
<div align="center">Select option 1 - SOcial-Engineering Attacks from the menu</div>
<p align="center"><img src=images/Picture8.png></p>
<div align="center">Select option 5 - Mass Mailer Attack from the menu</div>
<p align="center"><img src=images/Picture9.png></p>
<div align="center">Select option 1 - E-Mail Attack Single Email Address</div>
<p align="center"><img src=images/Picture10.png></p>
<div align="center">Select option 2 - One-Time Use Email Template</div>
<p align="center"><img src=images/Picture11.png></p>
<div align="center">Fill in all the information for the email</div>
<p align="center"><img src=images/Picture12.png></p>

---

***Step 4: Target View***
<div align="center">Email inbox view of target</div>
<p align="center"><img src=images/Picture13.png></p>
<div align="center">Email View with phishing link attached</div>
<p align="center"><img src=images/Picture14.png></p>
<div align="center">Phishing LinkedIn page once the link is clicked</div>
<p align="center"><img src=images/Picture15.png></p>
<div align="center">Target enters credential to login</div>
<p align="center"><img src=images/Picture16.png></p>

---

***Step 5: Attacker View***
<div align="center">Review Zphisher for harvested credentials</div>
<p align="center"><img src=images/Picture17.png></p>
<div align="center">Review /auth in Zphisher for credentials</div>
<p align="center"><img src=images/Picture18.png></p>
<div align="center">Display ip.txt content for harvested IP address</div>
<p align="center"><img src=images/Picture19.png></p>
<div align="center">Display usernames.dat content for harvested username and password</div>
<p align="center"><img src=images/Picture20.png></p>


## Preventive Measures

- ***Verify Email Source:*** Always check the sender's email address for authenticity. Be cautious of emails from unfamiliar sources or slightly alter known addresses.
- ***Look for Formatting and Language errors:*** Phishing emails often contain formatting issues or language errors. Attention to these details can be crucial indicator of a phishing attempt.
- ***Avoid Clicking on Suspicious Links:*** Be careful of clicking on links in unsolicited emails, especially those that prmpt for login credentials.
- ***Use of Two-Factor-Authentication (2FA):*** Implementing 2FA can add an extra layer of security, making it harder for attackers to gain access even if credentials are compromised.

## Conclusion

This project provided practical experience intergrating two different tools - Zphisher and SET - for an effective phishing attack. Zphisher was instrumental in creating a convincing LinkedIn phishing page that could clone the actual LinkedIn login page, allowing successful credential harvesting. SET's Mass Mailer Attack feature was utilized to distribute the phishing email containing the link created by Zphisher. This combination showcased how various tools can be complement each other in a social engineering context.

## Full Disclaimer

*Any action and or activities related to the material contained within this repository is solely your responsibility. The misuse of the tools and information in this repo could result in criminal charges being brought against the person in question. The author will not be held responsible in the event any criminal charges are brought against any individuals misusing the tools and information in this repository for malicious purpose or to break the law.*

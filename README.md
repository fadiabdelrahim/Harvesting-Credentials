# Harvesting-Credentials

## Introduction

In todays digital landscape, the threat of cyber-attacks, particularly through phishing, has become a signigicant concern for individuals and organizations alike. Phishing attacks, which often involve tricking individuals into revealing sensiitive information such as login credentaisl, continue to be a prevalant method emplyed by cybercriminals. 

This project delves into a specific instance of phishing simulation, showacsing teh user of sophisticated tools and techniques to harvest credentials. It aims to provide an in-depth analysis of a phishing scenario, where a LinkedIn-themed phishing attack was deployed to engage a target through professional networking channel. The choice of LinkedIn as the phishing template was strategic, given the platforms credibility and the likelihood of successful interaction by the target. 

Architecture of Harvesting Credentials

- Kali Linux - linux distribution designed for digital forensics and penetration testing
- Zphisher - a powerful open-source Phishing tool
- The Socail-Engineer Toolkit (SET) - an open-source penetration testing framework designed for social engineering.


## Choice of a Web Template

The LinkedIn template is chosen for its relevance to the pretexting scenario, which involves engaging with Dr. Alexander through professioanl networking. LinkedIn is a trusted platform for professionals and using this template in the phishing attack increases the likelihood of Dr. Alexander interacting with it.

## Step-by-Step Deployment

<b>Step 1:</b> Zphisher installation for Linux

![image](https://github.com/user-attachments/assets/20c5a156-df2c-4856-baf2-107ff6367268)

![image](https://github.com/user-attachments/assets/abfd2841-d84d-4edd-a944-b57ebba58416)

<b>Step 2:</b> Zphisher setup for LinkedIn Phishing page

- Select option [14] LinkedIn

![image](https://github.com/user-attachments/assets/27b824fd-e67e-4c09-a85b-8bb0c8de2c80)

- Select option [2] Cloudflard a port forwarding service

![image](https://github.com/user-attachments/assets/81657828-34c7-41ca-b5b5-a2b2cb2b0710)

- Select option N for do you want a custom port

![image](https://github.com/user-attachments/assets/4089e674-7e6e-4617-adf2-db0b2525de79)

- Copy URL 1 Link to use in SET to send the email

![image](https://github.com/user-attachments/assets/46e8c11e-4674-43f2-a901-a71807f78dfd)

<b>Step 3:</b> The Social-Engineer ToolKit (SET) setup to craft and send the phishing email 

- Run SET

![image](https://github.com/user-attachments/assets/e31fee7d-0989-4e66-8304-be973334436a)

- Select option 1 - SOcial-Engineering Attacks from the menu

![image](https://github.com/user-attachments/assets/84687065-c6ce-45c4-be05-c2f5cb7c63be)

- Select option 5 - Mass Mailer Attack from the menu

![image](https://github.com/user-attachments/assets/c9d34021-78bd-440d-a2b3-324fd91438de)

- Select option 1 - E-Mail Attack Single Email Address

![image](https://github.com/user-attachments/assets/fc496860-90d6-4d79-9ecf-9b0cda7573ec)

- Select option 2 - One-Time Use Email Template

![image](https://github.com/user-attachments/assets/83ae1595-0abd-4c72-8625-6969ed39382b)

- Fill in all the information for the email

![image](https://github.com/user-attachments/assets/ecbdc541-df5b-454d-b9ad-364f17587789)

<b>Step 4:</b> Target View

- Email inbox view of target

![image](https://github.com/user-attachments/assets/af62ef06-fbd9-4e28-9a14-af4ff3edfec6)

- Email View with phishing link attached

![image](https://github.com/user-attachments/assets/234613ca-1ad0-4528-9d75-3625467f26ed)

- Phishing LinkedIn page once the link is clicked

![image](https://github.com/user-attachments/assets/cb3289ef-8b90-48e5-9d99-ded46f3035d3)

- Target enters credential to login

![image](https://github.com/user-attachments/assets/668bfef6-60f7-444b-9f34-e030508ddf4d)

<b>Step 5:</b> Attacker View

- Review Zphisher for harvested credentials

![image](https://github.com/user-attachments/assets/71333e30-dbc5-4cdd-8b3b-e85cc92dcd1e)

- Review auth/ in Zphisher for credentials

![image](https://github.com/user-attachments/assets/fdce695b-5611-4a12-8560-c656b086621c)

- Display ip.txt content for harvested IP address

![image](https://github.com/user-attachments/assets/4ec7c7ea-e79e-4bf5-aaa8-9fd6fd0732df)

- Display usernames.dat content for harvested username and password

![image](https://github.com/user-attachments/assets/311716fe-8be8-4d2a-a064-e6aeb5aa2060)

## Preventive Measures

- <b>Verify Email Source:</b> Always check the sender's email address for authenticity. Be cautious of emails from unfamiliar sources or slightly alter known addresses.
- <b>Look for Formatting and Language errors:</b> Phishing emails often contain formatting issues or language errors. Attention to these details can be crucial indicator of a phishing attempt.
- <b>Avoid Clicking on Suspicious Links:</b> Be careful of clicking on links in unsolicited emails, especially those that prmpt for login credentials.
- <b>Use of Two-Factor-Authentication (2FA):</b> Implementing 2FA can add an extra layer of security, making it harder for attackers to gain access even if credentials are compromised.

## Conclusion

This project provided practical experience intergrating two different tools - Zphisher and SET - for an effective phishing attack. Zphisher was instrumental in creating a convincing LinkedIn phishing page that could clone the actual LinkedIn login page, allowing successful credential harvesting. SET's Mass Mailer Attack feature was utilized to distribute the phishing email containing the link created by Zphisher. This combination showcased how various tools can be complement each other in a social engineering context.

# Google Cybersecurity Professional - Yummy Recipes Company

## Table of contents

- [Overview](#overview)
  - [The objective](#the-objective)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Tools used](#tools-used)
  - [Achievement](#achievement)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

You are a cybersecurity analyst for yummyrecipesforme.com, a website that sells recipes and cookbooks. A disgruntled baker has decided to publish the website’s best-selling recipes for the public to access for free.

The baker executed a brute force attack to gain access to the web host. They repeatedly entered several known default passwords for the administrative account until they correctly guessed the right one. After they obtained the login credentials, they were able to access the admin panel and change the website’s source code. They embedded a javascript function in the source code that prompted visitors to download and run a file upon visiting the website. After running the downloaded file, the customers are redirected to a fake version of the website where the seller’s recipes are now available for free.

Several hours after the attack, multiple customers emailed yummyrecipesforme’s helpdesk. They complained that the company’s website had prompted them to download a file to update their browsers. The customers claimed that, after running the file, the address of the website changed and their personal computers began running more slowly.

In response to this incident, the website owner tries to log in to the admin panel but is unable to, so they reach out to the website hosting provider. You and other cybersecurity analysts are tasked with investigating this security event.

To address the incident, you create a sandbox environment to observe the suspicious website behavior. You run the network protocol analyzer tcpdump, then type in the URL for the website, yummyrecipesforme.com. As soon as the website loads, you are prompted to download an executable file to update your browser. You accept the download and allow the file to run. You then observe that your browser redirects you to a different URL, greatrecipesforme.com, which is designed to look like the original site. However, the recipes your company sells are now posted for free on the new website.

The logs show the following process:

- The browser requests a DNS resolution of the yummyrecipesforme.com URL.

- The DNS replies with the correct IP address.

- The browser initiates an HTTP request for the webpage.

- The browser initiates the download of the malware.

The browser requests another DNS resolution for greatrecipesforme.com.

The DNS server responds with the new IP address.

The browser initiates an HTTP request to the new IP address.

A senior analyst confirms that the website was compromised. The analyst checks the source code for the website. They notice that javascript code had been added to prompt website visitors to download an executable file. Analysis of the downloaded file found a script that redirects the visitors’ browsers from yummyrecipesforme.com to greatrecipesforme.com.

The cybersecurity team reports that the web server was impacted by a brute force attack. The disgruntled baker was able to guess the password easily because the admin password was still set to the default password. Additionally, there were no controls in place to prevent a brute force attack.

Your job is to document the incident in detail, including identifying the network protocols used to establish the connection between the user and the website.  You should also recommend a security action to take to prevent brute force attacks in the future.

### The objective

- Name one network protocol identified during the investigation

- Document the incident

- Recommend one security measure

### Screenshot

![dns & http traffic log image](../Image/DNS%20&%20HTTP%20traffice%20log.png)

### Links

[Document link]

- [Security Incident Report](https://docs.google.com/document/d/1C-EUcX16l8Jy1YKrL4NobS0yticPwZ_JxIYrnCPdgZk/edit?usp=drive_link&resourcekey=0-n24_QSC8zphpZWZ_fZ3qYQ)

- [DNS & HPPT Traffic Log](https://docs.google.com/document/d/1cybgKs-biF4SpiigCwdBicbOmCZ65LO8kx4OlLmGo4Y/edit?usp=drive_link&resourcekey=0-exso31cdETPGQSANGUXbgw)

## My process

After serveral complain from customer, I created a sandbox environment and run tcpdump network protocal analyer to observe the suspicious website behavior. while all tool are open for invesstigation I type the company URL [www.yummyrecipesforme.com](www.yummyrecipesforme.com) on the browser in the sandbox enviroment I created.

After the webpage load, it prompted me to download an excutable file to update my browser. I downloaded the file and run it, then I was redirected to a new differenct URL, [www.greatrecipesforme.com](www.greatrecipesforme.com) which look extract as the original website.

Investigation shows that the company website has been compromised, javascript code has been added to the website source code which prompt visitor to download an excutable file which redirect them to from [www.yummyrecipesforme.com](www.yummyrecipesforme.com) to [www.greatrecipesforme.com](www.greatrecipesforme.com)

This indicate a **brute force attack**, the incident was documented and security tips was provided to strenghting the security posture such as enabling multi-factor authentication, strong password policy, limit login attempt and installing IDS, IPS, SIEM tools and reconfigure firewall to filter unfamiliar IP address.

### Tools Used

- Wireshark

### Achievement

- Detected a malicious attack through DNS and HTTP traffic log analysis.
- Documentation of security incidents and causes of incident attack.
- Appling double layer security by implementing Multi-Factor Authentication/Two Ways Factor Authentication, strong password policy, Limit login attempt and Monitoring login activities.

### Useful resources

[How to read the DNS & HTTP traffic log](https://docs.google.com/document/d/1cybgKs-biF4SpiigCwdBicbOmCZ65LO8kx4OlLmGo4Y/edit?usp=drive_link&resourcekey=0-exso31cdETPGQSANGUXbgw)

[DNS & HTTP traffic log explained](https://docs.google.com/spreadsheets/d/1M8N9F6-TsW8Mx2VyW5z0DtGK4ZVNhdFl2hIojL12xMQ/edit?usp=drive_link)

## Author

[LinkedIn](www.linkedin.com/in/olagoke-holo)

[Facebook](https://web.facebook.com/olagoke.holo.3/)

[Twitter](https://twitter.com/olarragoken)

[Instagram](https://www.instagram.com/holoolagoke/)

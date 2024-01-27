# Google Cybersecurity Professional - Travel Agency Company

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Tools used](#tools-used)
  - [Achievement](#achievement)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

You work as a security analyst for a travel agency that advertises sales and promotions on the company’s website. The employees of the company regularly access the company’s sales webpage to search for vacation packages their customers might like.

One afternoon, you receive an automated alert from your monitoring system indicating a problem with the web server. You attempt to visit the company’s website, but you receive a connection timeout error message in your browser.

You use a packet sniffer to capture data packets in transit to and from the web server. You notice a large number of TCP SYN requests coming from an unfamiliar IP address. The web server appears to be overwhelmed by the volume of incoming traffic and is losing its ability to respond to the abnormally large number of SYN requests. You suspect the server is under attack by a malicious actor.

You take the server offline temporarily so that the machine can recover and return to a normal operating status. You also configure the company’s firewall to block the IP address that was sending the abnormal number of SYN requests. You know that your IP blocking solution won’t last long, as an attacker can spoof other IP addresses to get around this block. You need to alert your manager about this problem quickly and discuss the next steps to stop this attacker and prevent this problem from happening again. You will need to be prepared to tell your boss about the type of attack you discovered and how it was affecting the web server and employees.

### The challenge

- Reflect on the types of network intrusion attacks that you have learned about in this course so far. As a security analyst, identifying the type of network attack based on the incident is the first step to managing the attack and preventing similar attacks in the future.

        Here are some questions to consider when determining what type of attack occurred:

        - What do you currently understand about network attacks?

        - Which type of attack would likely result in the symptoms described in the scenario?

        - What is the difference between a denial of service (DoS) and distributed denial of service (DDoS)?

        - Why is the website taking a long time to load and reporting a connection timeout error?

- When writing your report, discuss the network devices and activities that are involved in the interruption. Include the following information in your explanation:

        - Describe the attack. What are the main symptoms or characteristics of this specific type of attack?

        - Explain how it affected the organization’s network. How does this specific network attack affect the website and how it functions?

        - Describe the potential consequences of this attack and how it negatively affects the organization.

        - Optional: Suggest potential ways to secure the network so this attack can be prevented in the future.

### Links

[Document link]

[Incident report](https://docs.google.com/document/d/1i6D4PJEMNbyiCAJvq3Y6cBmjCnHx8JG0ch7C5OZmbSE/edit?usp=drive_link)

[Wireshark TCP/HTTP log](https://docs.google.com/spreadsheets/d/1y7Np71rdEmfIuMeCRgQAzMd66xrK3QGZ2uvGyUwfkF4/edit?usp=drive_link)

## My process

After I received the alert of a problem with the comapny web server, I opened the company website but received a connection timeout error. I launched Wireshark to investigate the traffice incident.

I used packet sniffer to captured data packets in transit to and from the company web server. In the wireshark log result, I notice a large number of TCP SYN requests coming from 203.0.113.0 which is unfamiliar IP address. This has made the web server overwhelmed due to the volume of incoming traffic and losing it ability to respond to the abnormally large number of SYN reuest, this indicated a Denial of Service from a malicious actor because it coming from a single IP address.

I temporarily set the server offline to stop the SYN request caused from DoS so that the machine can recover and get back to it normal operation. I also configured the firewall to stop the specific IP address that cause DoS from assessing the company web server. I provided tip for securing the company entire network by properly configured the firewall to block unfamiliar IP address and install Anti-virus software.

### Tools Used

- Wireshark
- SIEM

### Achievement

- Detected  a Denial of Service attack using packet sniffer to read data packets transit.

- figured out type of attack and the IP address causing the attack.

- Configured the wirewall to block the IP address and any unfamiliar IP address in the future.

- Documented the security attack incident and its impact.

### Useful resources

[How to read a Wireshark TCP/HTTP log](https://docs.google.com/document/d/1PykdunzXsQ0dTZkczfdsehBXbJV5g10LuHqkOJz9oRw/edit?usp=drive_link)

## Author

[LinkedIn](www.linkedin.com/in/olagoke-holo)

[Facebook](https://web.facebook.com/olagoke.holo.3/)

[Twitter](https://twitter.com/olarragoken)

[Instagram](https://www.instagram.com/holoolagoke/)

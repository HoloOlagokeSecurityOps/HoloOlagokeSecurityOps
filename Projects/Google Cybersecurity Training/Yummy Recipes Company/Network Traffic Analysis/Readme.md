# Google Cybersecurity Professional - Yummy Recipes Company

## Table of contents

- [Overview](#overview)
  - [The objective](#the-objective)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Tools used](#tools-used)
  - [Achievement](#achievement)
- [Author](#author)

## Overview

You are a cybersecurity analyst working at a company that specializes in providing IT consultant services. Several customers contacted your company to report that they were not able to access the company website [www.yummyrecipesforme.com](www.yummyrecipesforme.com), and saw the error “destination port unreachable” after waiting for the page to load.

You are tasked with analyzing the situation and determining which network protocol was affected during this incident. To start, you visit the website and you also receive the error “destination port unreachable.” Next, you load your network analyzer tool, tcpdump, and load the webpage again. This time, you receive a lot of packets in your network analyzer. The analyzer shows that when you send UDP packets and receive an ICMP response returned to your host, the results contain an error message: “udp port 53 unreachable.”

### The objective

- Provide a summary of the problem found in the DNS and ICMP traffic log

- Explain your analysis of the data and provide one possible cause of the incident

### Screenshot

![network traffic log image](../Image/Network%20traffic%20log.png)

### Links

[Document link]

- [Cybersecurity Incident Report: Network Traffic Analysis](https://docs.google.com/document/d/1gvwQR5DRX-_E4_hUMjhW_3LUxEXwB_8G5nF9br3TUtQ/edit?usp=drive_link&resourcekey=0-nIu_GTk9V03mh-uMb-B-GA)

- [Network Traffic Log](https://docs.google.com/document/d/1lCLnx0bigOZwH0Jp8uUBx5O4Gy5yqxjQDc5GFo_XWko/edit?usp=drive_link)

## My process

After I received the downtime of the company server, I launched tcpdump analyzer to analyze the network traffic to know issue. I load the webpage again while reading the log, a lot of packets was displayed.
while connecting to IP address 203.0.113.2.domain it respond show an error message “udp port 53 unreachable”
This indicate that the company server has been attacked with ICPM flood.

### Tools Used

- Wireshark

### Achievement

- Reading network traffic log.
- Detected ICPM flood attack.
- Detected a malicious attack through DNS and HTTP traffic log analysis.
- Documentation of security incidents and causes of incident attack.
- Appling double layer security by implementing Multi-Factor Authentication/Two Ways Factor Authentication, strong password policy, Limit login attempt and Monitoring login activities.

## Author

[LinkedIn](www.linkedin.com/in/olagoke-holo)

[Facebook](https://web.facebook.com/olagoke.holo.3/)

[Twitter](https://twitter.com/olarragoken)

[Instagram](https://www.instagram.com/holoolagoke/)

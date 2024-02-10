# Google Cybersecurity Professional - Imaginary Bank
## Table of contents

- [Scenario](#scenario)
  - [The objective](#the-objective)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My approach](#my-approach)
  - [Achievement](#achievement)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Scenario

You’re a security analyst at an investment firm called Imaginary Bank. An executive at the firm recently received a spear phishing email that appears to come from the board of Imaginary Bank. Spear phishing is a malicious email attack targeting a specific user or group of users, appearing to originate from a trusted source. In this case, the executive is being asked to install new collaboration software, ExecuTalk.

The executive suspects this email might be a phishing attempt because ExecuTalk was never mentioned during the last board meeting. They've forwarded the message to your team to verify if it’s legitimate. Your supervisor has tasked you with investigating the message and determining whether it should be quarantined.

    ---------------mail content---------------

    From: imaginarybank@gmail.org

    Sent: Saturday, December 21, 2019  15:05:05

    To: cfo@imaginarybank.com

    Subject:  RE: You are been added to an ecsecutiv's groups

    Conglaturations! You have been added to a collaboration group ‘Execs.’

    Downlode ExecuTalk to your computer.

    Mac® | Windows® | Android™ 

    You're team needs you! This invitation will expire in 48 hours so act quickly.

    Sincerely,

    ExecuTalk©

    All rights reserved.

### The objective

- Which two clues in the message header indicate to you that this is a phishing attempt?

- What details make this message appear legitimate?

- The download options open a webpage that contains a login form where someone can enter a username and password. Carefully review the webpage. What is the main clue that indicates this form is malicious?

- After completing your investigation, should this email be quarantined?

### Screenshot

![Mail content](./Image/Imaginary%20bank%20mail.png)

![Download page](./Image/Imaginary%20bank%20login%20form.png)

### Links

  [Document link]

[Filter malicious emails](https://docs.google.com/document/d/1G4S0qJMaXDcl-ekLh9LbzPQO1iu-jjcL959l9nOud60/edit?usp=sharing)

## My approach

The mail was opened in a VM workstation for investigation. I opened the mail, the header of the mail indicated that the mail is a phishing attempt because the sender use a different domain which is "@gmail.com" instead of "@imaginarybank.com", the "RE:" in the email subject indicated that it is a reply message and it contains many grammatical error. Which indicated the mail is coming from threat actor.

Though, the download options, title group, brand and labeling make the body of the mail appear legitimate but the the download page does not support HTTPS encryption which does not make it a secure site. The URL of the download page used a different domain and it required me to login my credential which is not advisable to do such thing on unknown or unsecured website. So, I ignored the action and documented the incident.

### Achievement

- Documented an investigation on malicious email.
- Identified suspicious anomalies on the mail header.

### Useful resources

[security tips on using caution with USB drives](https://www.cisa.gov/news-events/news/using-caution-usb-drives)

## Author

[LinkedIn](www.linkedin.com/in/olagoke-holo)

[Facebook](https://web.facebook.com/olagoke.holo.3/)

[Twitter](https://twitter.com/olarragoken)

[Instagram](https://www.instagram.com/holoolagoke/)

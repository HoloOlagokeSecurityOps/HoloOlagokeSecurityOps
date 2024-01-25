# Google Cybersecurity Professional - Installation in Linux OS

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Tools used](#tools-used)
  - [Achievement](#achievement)
- [Author](#author)

## Overview

Your role as a security analyst requires that you have the Suricata and tcpdump network security applications installed on your system.

In this scenario, you have to install, uninstall, and reinstall these applications on your Linux Bash shell. You also need to confirm that you’ve installed them correctly.

Here’s how you'll do this: First, you’ll confirm that APT is installed on your Linux Bash shell. Next, you’ll use APT to install the Suricata application and confirm that it is installed. Then, you’ll uninstall the Suricata application and confirm this as well. Next, you’ll install the tcpdump application and list the applications currently installed. Finally, you’ll reinstall the Suricata application and confirm that both applications are installed.

### The challenge

- Confirm APT is installed in Bash

- Install Suricata with APT

- Uninstall Suricata with APT

- Install tcpdump with APT

- Reinstall Suricata with APT

### Screenshot

![apt command line](../Image/Installation/apt%20command%20line.png)

![install sunicata](../Image/Installation/install%20suricata.png)

![confirm installation of sunicata](../Image/Installation/confirm%20suricata%20installation.png)

![uninstall sunicata](../Image/Installation/uninstall%20suricata.png)

![install tcpdump](../Image/Installation/install%20tcpdump.png)

![list install app](../Image/Installation/list%20installed%20app.png)

### Links

[Document link]

- [App installation in Linux](https://docs.google.com/document/d/1JOGUeJNNfQvdiyITz1f7-QJQo77roo-5wxFXc9m3kn8/edit?usp=drive_link)

## My process

I used ``` apt ``` command  to ensure that Advanced Package Tool is installed.

I used ``` sudo apt install suricata ``` to install suricata on the machine, then I used ``` suricata ``` to ensure the app has been installed successfully, finally I used ``` sudo apt remove suricata ``` to uninstall suricata app from the machine and type ``` suricata ``` to ensure the app is successfully uninstalled.

I installed tcpdump using ``` sudo apt install tcpdump ```.

I used ``` sudo apt list --install ``` to view all installed app on the Linux machine.

### Tools Used

- Linux OS

### Achievement

- ensure an app is using the app name ``` apt ```.

- installed app on the machine using the ``` sudo ``` as root privilege with ``` apt install ``` and ``` suricata ``` the app name.

- uninstall an app using ``` sudo apt remove suricata ```.

- view app installed on the machine using ``` sudo apt list --install ```.

## Author

[LinkedIn](www.linkedin.com/in/olagoke-holo)

[Facebook](https://web.facebook.com/olagoke.holo.3/)

[Twitter](https://twitter.com/olarragoken)

[Instagram](https://www.instagram.com/holoolagoke/)

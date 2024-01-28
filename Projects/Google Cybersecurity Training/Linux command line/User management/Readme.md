# Google Cybersecurity Professional - Add and Manage user in Linux OS

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

In this scenario, a new employee with the username researcher9 joins an organization. You have to add them to the system and continue to manage their access during their time with the organization.

Here’s how you’ll do this task: First, you’ll add a new employee to the system and then to their primary group. Second, you’ll make this employee the owner of a file related to a particular project. Third, you’ll add the new employee to a supplementary group. Finally, you’ll delete the employee from the system.

### The objective

- Add a new employee

- Change ownership of a file

- Add the new employee to a new group

- Delete the employee from the system

### Screenshot

![useradd command line](../Image/Manage%20authorization/useradd.png)

![chown command line](../Image/Manage%20authorization/chown.png)

![usermod command line](../Image/Manage%20authorization/usermod.png)

![userdel command line](../Image/Manage%20authorization/userdel.png)

### Links

[Document link]

- [Add and Manage User in Linux](https://docs.google.com/document/d/1aChVIUYe0wAcs3NSJngL8JWF6FeuouI5gCUIA0LqdCw/edit?usp=drive_link)

## My process

I used the following command line to add a new user system.

```bash

sudo useradd researcher9 # add a user called researcher9 to the system

sudo usermod -g research_team researcher9 # add the user called researcher9 to a group called research_team

```

I used the following command line to assign a file to researcher9.

```bash

cd /home/researcher2/projects # navigate to projects directory

sudo chown researcher9 project_r.txt # change the ownership of project_r.txt file to researcher9

ls -l # to confirm if the operation was successful

```

I used the following command line to add researcher9 to sales team.

```bash

sudo usermod -aG sales_team researcher9 # add  researcher9 to another group called sales_team. -a is used to ensure that user researcher9 is added to sales_team without been remove from research_team, G is used to add a user to secondary group

```

I used the following command line to remove researcher9 from the system.

```bash

sudo userdel researcher9 # remove user researcher9 from the system. the operation was not successful because the user is the only member of that group. Then the next command line was used

sudo groupdel researcher9 # remove user researcher9 and the empty group

```

### Tools Used

- Linux OS
- Bash

### Achievement

- used ``` useradd ``` command to add a user to the system.

- used ``` usermod ``` command with ``` -g ``` to add a user to primary group.

- used ``` chown ``` command to assign file ownership to a user.

- used ``` usermod ``` command with ``` -aG ``` to add a user to secondary group.

- used ``` userdel ``` command to remove a user to the system.

- used ``` groupdel ``` command to remove a group to the system.

## Author

[LinkedIn](www.linkedin.com/in/olagoke-holo)

[Facebook](https://web.facebook.com/olagoke.holo.3/)

[Twitter](https://twitter.com/olarragoken)

[Instagram](https://www.instagram.com/holoolagoke/)

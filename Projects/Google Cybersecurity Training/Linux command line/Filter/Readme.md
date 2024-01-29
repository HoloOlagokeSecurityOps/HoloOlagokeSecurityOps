# Google Cybersecurity Professional - Filter a file in Linux OS

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

In this scenario, you need to obtain information contained in server log and user data files. You also need to find files with specific names.

Here’s how you’ll do this: First, you’ll navigate to the logs directory and return the error messages in the server_logs.txt file. Next, you’ll navigate to the users directory and search for files that contain a specific string in their names. Finally, you’ll search for information contained in user files.

### The objective

- Search for error messages in a file

- Search for files that contain a specific string

- Search for information in user files

### Screenshot

![grep-directory command line](../Image/Manage%20files/grep%20directory.png)

![pipe command line](../Image/Manage%20files/pipe.png)

![grep-file command line](../Image/Manage%20files/grep%20file.png)

### Links

[Document link]

- [Filter a file in Linux](https://docs.google.com/document/d/12M2mXg9gwTNTVOmy-DHB4CIrDx5kMhY526VE5EHLBAQ/edit?usp=drive_link)

## My process

I used the following command line to serach server_logs.txt for error string.

```bash

pwd # display my current directory

cd /home/analyst/logs # navigate to logs directory

ls # list the items in the directory

grep "error" server_logs.txt # search for error string in the server_logs.txt file

```

I used the following command line to serach through users directory for file that filename consist "Q1" and file that filename consist "access".

```bash

cd /home/analyst/reports/users # navigate to users directory

ls /home/analyst/reports/users | grep "Q1" # search for file that filename consist Q1 in the user directory

ls /home/analyst/reports/users | grep "access" # search for file that filename consist access in the user directory

```

I used the following command line to serach deleted users in Q2_deleted_users.txt and users added to Human Resources department in Q4_added_users.txt.

```bash

grep "jhill" Q2_deleted_users.txt # search for jhill record in the Q2_deleted_users.txt file

grep "Human Resources" Q4_added_users.txt # search for user add to the Human Resources department in the Q2_added_users.txt file

```

### Tools Used

- Linux OS
- Bash

### Achievement

- used ``` grep ``` command  display string in the bash shell.

- used ``` pipe ``` command ``` grep ``` command to perform some nathematical calculations.

## Author

[LinkedIn](www.linkedin.com/in/olagoke-holo)

[Facebook](https://web.facebook.com/olagoke.holo.3/)

[Twitter](https://twitter.com/olarragoken)

[Instagram](https://www.instagram.com/holoolagoke/)

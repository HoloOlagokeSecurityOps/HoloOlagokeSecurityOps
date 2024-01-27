# Google Cybersecurity Professional - Manage files in Linux OS

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

In this scenario, you need to ensure that the /home/analyst directory is properly organized.

You have to make a few changes to the /home/analyst directory and the files it contains.

You also have to edit a file to record the changes or updates you make to the directory.

When you start, the /home/analyst directory contains the following subdirectories and files:

    home
    └── analyst
        ├── notes
        │   ├── Q3patches.txt
        │   └── tempnotes.txt
        ├── reports
        │   ├── Q1patches.txt
        │   └── Q2patches.txt
        └── temp

You need to modify the /home/analyst directory to the following directory and file structure:

    home
    └── analyst
        ├── logs
        ├── notes
        │   └── tasks.txt
        └── reports
            ├── Q1patches.txt
            └── Q2patches.txt
            └── Q3patches.txt

Here’s how you’ll do this: First, you’ll create a new subdirectory called logs in the /home/analyst directory. Next, you’ll remove the temp subdirectory. Then, you’ll move the Q3patches.txt file to the reports subdirectory and delete the tempnotes.txt file. Finally, you’ll create a new .txt file called tasks in the notes subdirectory and add a note to the file describing the tasks you've performed.

You’ll need to use the commands learned in the video lesson to complete these steps.

### The challenge

- Create a new directory

- Remove a directory

- Move a file and delete a file

- Create a file and add text using nano

### Screenshot

![mkdir command line](../Image/Manage%20files/mkdir.png)

![rmdir command line](../Image/Manage%20files/rmdir.png)

![mv command line](../Image/Manage%20files/mv.png)

![rm command line](../Image/Manage%20files/rm.png)

![touch command line](../Image/Manage%20files/touch.png)

![nano command line](../Image/Manage%20files/nano.png)

### Links

[Document link]

- [Manage files in Linux](https://docs.google.com/document/d/1m6VMXOVFDKZXI28ILJ_JOekLq1hPPyAMqsZ4Y38y14Q/edit?usp=drive_link)

## My process

I used the following command line to create a directory.

```bash

pwd # display my current directory

ls # list the items in the directory

sudo mkdir logs # create a directory called logs

ls # list the items again to confirm my action

```

I used the following command line to delete a directory.

```bash

ls # list the items in the directory

sudo rmdir temp # delete a directory called temp

ls # list the items again to confirm my action

```

I used the following command line to move a file to another directory.

```bash

ls # list the items in the directory

sudo mv Q3patches.txt /home/analyst/reports # move a file named Q3patches.txt to reports directory

ls # list the items again to confirm the file has been moved

cd /home/analyst/reports # change my current directory to reports directory

ls # list the items in the reports directory to confrimed the file has been moved here

```

I used the following command line to delete a file.

```bash

cd /home/analyst/notes # change my current directory to notes directory

ls # list the items in the directory

sudo rm tempnotes.txt # delete a file named tempnotes.txt

ls # list the items again to confirm the file has been deleted

```

I used the following command line to create a file.

```bash

cd /home/analyst/notes # change my current directory to notes directory

ls # list the items in the directory

sudo touch tasks.txt # create a file named tasks.txt

ls # list the items again to confirm the file has been created

```

I used the following command line to edit the file.

```bash

cd /home/analyst/notes # change my current directory to notes directory

ls # list the items in the directory

sudo nano tasks.txt # open tasks.txt in nano text editor

```

### Tools Used

- Linux OS
- bash

### Achievement

- used ``` pwd ``` command  display the directory I am working on.

- used ``` cd ``` command with the file path to change my directory location.

- used ``` ls ``` command to list the contents in a directory.

- used ``` cat ``` command to display a file contents.

- used ``` mkdir ``` command to create a directory.

- used ``` rmdir ``` command to delete a directory.

- used ``` mv ``` command to move a file to another directory.

- used ``` rm ``` command to delete a file.

- used ``` touch ``` command to create a file.

- used ``` nano ``` command to open a text editor.

## Author

[LinkedIn](www.linkedin.com/in/olagoke-holo)

[Facebook](https://web.facebook.com/olagoke.holo.3/)

[Twitter](https://twitter.com/olarragoken)

[Instagram](https://www.instagram.com/holoolagoke/)

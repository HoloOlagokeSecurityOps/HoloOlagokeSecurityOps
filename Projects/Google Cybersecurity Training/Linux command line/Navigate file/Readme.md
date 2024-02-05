# Google Cybersecurity Professional - Navigate files in Linux OS

## Table of contents

- [Scenario](#scenario)
  - [The objective](#the-objective)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My approach](#my-approach)
  - [Tools used](#tools-used)
  - [Achievement](#achievement)
- [Author](#author)

## Scenario

In this scenario, you have to locate and analyze the information of certain files located in the /home/analyst directory.

Here’s how you’ll do this: First, you’ll get the information of the current working directory you’re in and display the contents of the directory. Second, you’ll navigate to the reports directory and list the subdirectories it contains. Third, you’ll navigate to the users subdirectory and display the contents of the Q1_added_users.txt file. Finally, you’ll navigate to the logs directory and display the first 10 lines of a file it contains.

To complete these tasks, you'll need to use commands that you've previously learned in this course. Well, it's time to practice what you’ve learned. Let’s do this!

### The objective

- Find your current working directory and display its contents

- Navigate to a directory and list subdirectories

- Display the contents of a file

- Display the first 10 lines of a file

### Screenshot

![pwd command line](../Image/Navigate%20file/pwd.png)

![cd command line](../Image/Navigate%20file/cd.png)

![ls command line](../Image/Navigate%20file/ls.png)

![cat command line](../Image/Navigate%20file/cat.png)

![head command line](../Image/Navigate%20file/head.png)

### Links

[Document link]

- [Navigate files in Linux](https://docs.google.com/document/d/1PYGY1tX9rkLaWHGJR2thcL8pXZFsDnZOyWDqeW1-NGQ/edit?usp=drive_link)

## My approach

I used ``` pwd ``` command  display the directory I am working on. I used ``` cd ``` command with the file path ```/home/analyst/reports``` to  change my directory location from analyst to reports directory, I then used ``` ls ``` command to list the contents in the reports directory.

To read a file content using the command line the following command lines were used.

```bash

cd /home/analyst/reports/users # change my directory location from reports to users directory.

ls # display directory contents, 2 files was found.

cat Q1_added_users.txt #  display the file content.

```

To read 10 lines of a file content using the command line the following command lines were used.

```bash

cd /home/analyst/logs # change my directory location from users to logs directory.

ls # display directory contents, 1 file was found.

head server_logs.txt #  display 10 lines of the file content.

```

### Tools Used

- Linux OS
- Bash

### Achievement

- used ``` pwd ``` command  display the directory I am working on.

- used ``` cd ``` command with the file path to change my directory location.

- used ``` ls ``` command to list the contents in a directory.

- used ``` cat ``` command to display a file contents.

- used ``` head ``` command to display 10 lines of a file contents.

## Author

[LinkedIn](www.linkedin.com/in/olagoke-holo)

[Facebook](https://web.facebook.com/olagoke.holo.3/)

[Twitter](https://twitter.com/olarragoken)

[Instagram](https://www.instagram.com/holoolagoke/)

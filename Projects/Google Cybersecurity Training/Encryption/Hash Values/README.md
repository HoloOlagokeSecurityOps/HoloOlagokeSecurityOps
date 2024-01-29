objective# Google Cybersecurity Professional - Create Hash Values in Linux OS

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

In this scenario, we need to investigate whether two files are identical or different.

Here’s how you'll do this task: First, you’ll display the contents of two files and create hashes for each file. Next, you’ll examine the hashes and compare them.

Let’s hash some files!

### The challenge

- List the contents of the home directory

- Compare the plain text of the two files presented for hashing

- Compute the sha256sum hash of the two separate files

- Compare the hashes provided to identify the differences

### Screenshot

![sha256sum command](../Image/create%20hash%20value.png)

![cmp command](../Image/compare%20hash%20value.png)

### Links

[Document link]

- [create hash values in Linux](https://docs.google.com/document/d/1onM2DhPL2eNFZG-FRr6h4CESSyDVqQMjcf6gPX3i1FE/edit?usp=drive_link)

## My process

To created hash value for each file, I used the following command line

```bash

ls # display directory content

cat file1.txt # display file1 content

cat file2.txt # display file2 content

# Both of the file content are identical

sha256sum file1.txt # create hash value for file1 using sha256sum

sha256sum file2.txt # create hash value for file2 using sha256sum

```

To compare the hash value for each filse, I used the following command line

```bash

sha256sum file1.txt >> file1hash # create a new named file1hash and save file1.txt hash value in it

sha256sum file2.txt >> file2hash # create a new named file2hash and save file2.txt hash value in it

# Both of the file hash values are differ at the first character in the first line

```

### Tools Used

- Linux OS
- Bash

### Achievement

- use ``` sha256sum ``` to create hash value
- use ``` cmp ``` to compare hash value of two different files

## Author

[LinkedIn](www.linkedin.com/in/olagoke-holo)

[Facebook](https://web.facebook.com/olagoke.holo.3/)

[Twitter](https://twitter.com/olarragoken)

[Instagram](https://www.instagram.com/holoolagoke/)

# Google Cybersecurity Professional - Decrypt an Encrypted File in Linux OS

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

In this scenario, all of the files in your home directory have been encrypted. You’ll need to use Linux commands to break the Caesar cipher and decrypt the files so that you can read the hidden messages they contain.

Here’s how you’ll do this task: First, you’ll explore the contents of the home directory and read the contents of a file. Next, you’ll find a hidden file and decrypt the Caesar cipher it contains. Finally, you’ll decrypt the encrypted data file to recover your data and reveal the hidden message.

OK, it's time to decrypt some messages in Linux!

### The objective

- List the contents of a directory

- Read the contents of files

- Use Linux commands to revert a classical cipher back to plaintext

- Decrypt an encrypted file and restore the file to its original state



### Screenshot

![step 1](../Image/step%201.png)

![step 2](../Image/step%202.png)

![step 3](../Image/step%203.png)

### Links

[Document link]

- [Decrypt an encrypted message in Linux](https://docs.google.com/document/d/1uyldNPjUKQ_8dekm4EsdSwbpUxr1QneHtUooSOualUw/edit?usp=drive_link)

## My approach

I used ``` ls ``` command to display the content of my current directory, I found one directory named caesar, and two files; an encrypted file Q1.encrypted and a README.txt file that contain a guideline to decrypt the encrypted file.

I used ``` cd caesar``` to navigate to caesar directory, then, I used ``` ls -a ``` to display the hidden file. I used ``` cat .leftShift3 ``` to display the file content and found out it has been encrypted,  I used the ``` cat .leftShift3 | tr "d-za-cD-ZA-C" "a-zA-Z" ``` caesar cipher code to decrypt the file.
After I decrypted the file, the file content contain a decryption code for Q1.encrypted file.

I used ``` cd ~ ``` to navigate to home directory where Q1.encryption file is, I enter the used the decryption code I obtained from the previous decrypted file (.leftShift3) which is ``` openssl aes-256-cbc -pbkdf2 -a -d -in Q1.encrypted -out Q1.recovered -k ettubrute ```.
After I enter the code the Q1.encrypted file was decrypted with a new file named Q1.recovered.

### Tools Used

- Linux OS
- Bash

### Achievement

- decrypted a file using the command ``` tr "d-za-cD-ZA-C" "a-zA-Z" ``` translates all the lowercase and uppercase letters in the alphabet back to their original position.

- also used ``` openssl aes-256-cbc -pbkdf2 -a -d -in Q1.encrypted -out Q1.recovered -k ettubrute ``` command to decryoted and recover an encrypted file.

## Author

[LinkedIn](www.linkedin.com/in/olagoke-holo)

[Facebook](https://web.facebook.com/olagoke.holo.3/)

[Twitter](https://twitter.com/olarragoken)

[Instagram](https://www.instagram.com/holoolagoke/)

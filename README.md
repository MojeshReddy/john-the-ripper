# john-the-ripper
ohn the Ripper is a powerful, open-source password cracking software tool originally developed for Unix-based systems. It is widely used for both security auditing and penetration testing to identify weak passwords. This repository provides the latest versions of John the Ripper, along with essential updates and security patches. 
Introduction to John the Ripper:
John the Ripper is a tool used for cracking passwords, known for its speed and efficiency.
It works by decrypting passwords converted into hash forms using various algorithms.

 Understanding Hash Algorithms:
Different algorithms produce distinct hashes for the same password.
The tutorial uses browserling.com to demonstrate how a single password can have different hashes.

 Setting Up in Kali Linux:
The tutorial is demonstrated on Kali Linux.
It begins with opening a terminal window and gaining root access.


 Locating Passwords:
Passwords are located in the /etc/shadow file in hash format.
The tutorial shows how to view accounts and their corresponding hashed passwords.

 Creating Test Users:
Demonstrates adding new users (user1) and setting passwords for them.
These new accounts are then visible in the /etc/shadow file.

 Preparing for Password Cracking:
A copy of the /etc/shadow file is made and edited to include only the user1 account.
The file is saved as pass.txt for use with John the Ripper.

 Cracking Passwords:
The command john --format=crypt pass.txt is used to start cracking passwords.
John the Ripper identifies the passwords for both test accounts.

 Verifying Cracked Passwords:
The command john --show pass.txt confirms that the password have been cracked successfully.


# P2 - Passwords
Java program that reads a linux password file and uses a few different brute force methods to decrypt the password using JCrypt.

The salt is taken for each user individually and combined with the hash to be used for comparison. Using JCrypt, potential passwords
are encrypted and compared to each user's unique salt. If a match is found, the plaintext password is printed to the console. 

The username, first name, and last name are all encrypted first to see if they are the password. If not, these strings are mangled
using a variety of methods. 

After that point, a dictionary attack is used with the same string mangles. Users are skipped if the password can't be found with the
current implemented string mangles.

2nd Project for CS430 - Cybersecurity

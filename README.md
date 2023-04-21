# Vigenere Cipher Encryptor
Encryptor which uses the Vigenère cipher. This also adds another step to said cipher which I'm going to explain later.
## How it works
This program uses the Vigenère cipher. To use said cipher, we nees the message to be encrypted and a key, then  we substitute each letter with another, using your key to find the intersection of the correct row and column. For example, if it messages HELLO, you encrypt the first letter H using row H. Then you use the first letter of your key to choose the correct column. In this program however, we assign a letter with a number from 0 to 25. Then, to encrypt, write your message on one row (letters 0 – 25), and repeatedly write the keyword below it, adding each column, taking the result mod 26. These resultant numbers are the ciphertext. Here's an example:
```
Message: LETSGOTOTHESHOW     11 4 19 18 6 14 19 14 19  7 4 18  7 14 22
Key: TICKET                  19 8  2 10 4 19 19  8  2 10 4 19 19  8  2
Add:                        30 12 21 28 10 33 38 22 21 17 8 37 26 22 24
Mod:                          4 12 21 2 10 7 12 22 21 17 8 11 0 22 24
Ciphertext:                        E M V C K H M W V R I L A W Y
```
Here is the visualization of the cipher: (https://cdn-wordpress-info.futurelearn.com/info/wp-content/uploads/1.9Vignere1-1-768x512.png)

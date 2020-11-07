# Password-Checker
A password checker program in Python

The program uses requests, hashlib and sys Python modules.
Via the hashlib modul, the password we'd like to check is being hashed, using the sha1 hashing function. After that the hashed sequence is divided in 2 parts -
the first 5 and the rest of the symbols respectively. This is so it cannot be recognized once send over the internet for checkup. Then, only the first part is
being sent over to api.pwnedpasswords.com to check if it maches any leaked passwords on the site. All the passwords which match that part are being sent to us
as a response. After that the program continue the checkup on our computer, by adding the second part of the hashed password. At the end we get a result has 
our password been hacked ever, or not. We can also check multiple passwords at once.

The program can be run in a command prompt and also needs Python interpreter installed. 

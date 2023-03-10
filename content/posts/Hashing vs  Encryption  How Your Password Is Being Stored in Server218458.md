---
title: "Is Your Password Safe? Discover the Shocking Truth About Hashing Vs Encryption on Server Storage!"
ShowToc: true 
date: "2023-01-14"
author: "Laura Marlatt"
---
*****
Is Your Password Safe? Discover the Shocking Truth About Hashing Vs Encryption on Server Storage!

Do you know how safe your password is when stored on a server? It's important to understand the difference between hashing and encryption, and how they are used to safeguard your credentials. In this article, we'll explore the two methods and discover their strengths and weaknesses.

Hashing and encryption are two common techniques used to protect data. Hashing is a one-way process of turning data into a fixed-length string of characters. This string is then stored in a database or server, and can't be reversed back into its original format. Encryption, on the other hand, is a process of converting data into a format that can be read only by authorized users. In other words, encryption protects data by scrambling it so that only authorized individuals can read it.

When it comes to password storage on a server, hashing is the preferred method. Hashing passwords ensures that they can't be retrieved in readable format, even by someone with access to the server. This makes it more difficult for hackers to steal passwords and gain access to your accounts.

But not all hashing algorithms are created equal. Some are more secure than others. A good hashing algorithm should be both difficult to reverse engineer and resistant to collision attacks. Collision attacks occur when two different inputs result in the same hash output. This makes it possible for someone to guess your password even if they don't know the exact characters you used.

SHA-256 and bcrypt are two common hashing algorithms used by websites and servers to store passwords. SHA-256 is a widely used hashing algorithm that creates a 256-bit hash output. It's considered very secure and is used by many large companies to store sensitive data. Bcrypt is another popular hashing algorithm known for its additional security measures that include a salt value and work factor. This makes it more secure than SHA-256 and harder to crack through brute force attacks.

So, what about encryption? While encryption is great for protecting data in transit, it's not ideal for storing passwords on a server. Encryption requires a key to decrypt the data, which means that the key needs to be in a separate, secure location. In password storage, there isn't necessarily another separate, secure location to store that key. Plus, the decrypted password could still be stolen if someone gains access to the key.

In conclusion, always make sure you're using a site or service that stores passwords in a safe and secure manner. Always use strong, unique passwords, and enable two-factor authentication wherever possible. Remember, there's no such thing as 100% secure – but by following best practices, you can make it much harder for hackers to get their hands on your sensitive information.

{{< youtube qgpsIBLvrGY >}} 



Let’s say you set up an account at VerySecureWebsite.com. You type in your email address and password and set up your account. A little while later you receive an email informing you that, ironically, the website has been hacked, and the usernames and passwords of every user, which were stored in plaintext, are now for sale on the dark web. While you start changing the password on all your accounts (you only use one, you monster), you wonder, “Isn’t that a bad idea? Shouldn’t my password be in some kind of secret code so hackers can’t just read it?”
 
You’re correct. Any web app or service that uses a username/password login system should be storing their users’ passwords using a salted hash, possibly even a salted slow hash, perhaps with a pepper. If this is starting to sound more like breakfast than cryptography, don’t worry: unlike your password (hopefully), secure password storage isn’t too difficult of a topic to crack.
 
## Plaintext and basic encryption
 

 
Storing plaintext passwords in an Internet-connected database is a pretty bad idea: if the database gets hacked, anyone who has reused one of those passwords is now at risk. And yet a disturbing number of websites still do it, probably because security upgrades are more for the customer than the company. If you want to test whether a site is doing this, try selecting the “forgot password” option. If they just send you your password instead of a reset link, it’s being stored in plaintext.
 
Encryption may sound like a strong way to store passwords, but it’s really just a step above plaintext. An encrypted password can generally be decoded with a key, and if the hackers can find or guess it, the encryption is useless.
 
## Hashing > encryption
 
A hash function is basically just one-way encryption: you convert the plaintext password to a secret code, but there’s no key to convert it back, meaning you can never derive the actual password from the hashed version.
 
This is how most secure websites manage their passwords:
 
- The user creates an account
 - The user’s password is run through the hash function and stored in the database
 - Every time the user logs in, the database hashes the password they entered and checks to see if the entered hash matches the hash they have on file.
 - If yes, the user can log in

 
With a hash, the app/site never stores your actual password anywhere, and a hacker who breaks in will only get a list of letters and numbers that can’t be decoded. Depending on how strong the algorithm is, these hashes can be pretty difficult to crack.
 
Hashes aren’t hackproof, though. All an attacker has to do is run a dictionary of potential passwords through the hash function, then compare those hashes to the hashes in the database. When two hashes match, the hacker can just look at which password generated that hash.
 
To save time and computing power, many attackers just use a lookup table (or a “rainbow table,” a space-saving version of lookup tables), a pre-generated table full of potential passwords and their hashes. You can actually try hashing a plaintext word and then use a lookup table on the hash yourself; it’s not too hard. Essentially, if your password is at all common, the hash of that password is probably already in a lookup table. This is a great reason not to use common passwords.
 
## Salted hashes > hashes
 
Unlike slugs, salt makes hashes stronger. Since the entire hash changes even if just one letter of the plaintext word is changed, all a site needs to do to foil lookup tables is add some extra plaintext to the password before it’s hashed. The attacker will be able to read the plaintext salt since it’s stored in the database, but it forces them to recompute every possible combination of potential passwords and salts.
 
Of course, salted hashes can still be cracked. Hackers can just add the salt to the password they’re guessing, hash the combination, and wait for matches to pop up – a standard dictionary attack. Since modern GPUs can make billions of guesses per second, this isn’t at all infeasible, but it does make the process a lot more annoying. Failing that, brute-force attacks are slow but very effective.
 
## Making hashes even stronger: other tactics
 
Slow hashing algorithms, like PBKDF2 or bcrypt, use a technique known as “key stretching” to slow down dictionary and brute force attacks. This essentially involves setting the hash function to iterate a certain number of times (though it’s a bit more complex than just running the same thing over and over again), so that in order to reach the correct hash you have to use a lot of computing power. If a site is doing all this, their security is pretty good.
 
For added security, you can also “pepper” your hashes – which hopefully are already salted. A pepper, like a salt, is a set of values attached to the password before it is hashed. Unlike a salt, however, there is only one pepper value, and it is kept secret, separate from the salts and hashes. It adds another layer of security to the salted hash, but if the attacker manages to find it, it’s no longer very useful since the attacker can just use it to compute new lookup tables.
 
## Don’t make a hash of your hash
 
Password security has made some big advances – and so has the art of cracking that security. Unfortunately, humans are still bad at password management, and databases don’t upgrade security as often as they should. In general, assume that whenever you create an account, the password is being stored with relatively weak security. If your password is common or a dictionary word, then it’s at a pretty high risk of being cracked. Make your passwords long, mixing letters, numbers, and symbols, and you’ll be helping hash functions do their best work.
 
Image credits: Hash function
 
Andrew Braun is a lifelong tech enthusiast with a wide range of interests, including travel, economics, math, data analysis, fitness, and more. He is an advocate of cryptocurrencies and other decentralized technologies, and hopes to see new generations of innovation continue to outdo each other.
 
Our latest tutorials delivered straight to your inbox





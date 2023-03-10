---
title: "Stop Hackers In Their Tracks: Learn How To Secure Your Wordpress Passwords With Bcrypt Algorithm"
ShowToc: true 
date: "2023-06-18"
author: "Robert Corf"
---
*****
Stop Hackers In Their Tracks: Learn How To Secure Your WordPress Passwords With Bcrypt Algorithm

As the world becomes more digital, the issue of online security continues to be a critical concern for businesses and individuals. Hackers are getting smarter and more sophisticated in their attack methods, making it necessary for individuals to take strong measures to protect their online accounts. WordPress, one of the world's most popular content management systems, is particularly vulnerable to attacks, with hackers frequently attempting to gain access to user passwords.

One of the most effective ways of keeping your WordPress password safe is by using the Bcrypt algorithm. This article explores what the Bcrypt algorithm is, how it works, and how it can help secure your WordPress passwords.

What is the Bcrypt Algorithm?

Bcrypt is a password-hashing function used to encrypt passwords in a way that makes it challenging for hackers to decrypt them. It was designed as a defense against password cracking algorithms like brute force attacks, that attempt to guess a user's password using a systematic trial-and-error approach.

How Does Bcrypt Work?

At its core, Bcrypt works by taking a password and a "salt" value (an arbitrary number chosen to add complexity to the hash) and then hashing them together. The result is a string of letters and numbers that can be compared to other hashed passwords to determine whether the password entered is valid. However, unlike other hashing functions like MD5, Bcrypt is designed to be computationally intensive, which makes it challenging for attackers to decrypt the hash.

Why Use Bcrypt?

Bcrypt is a wise choice for WordPress passwords because it offers robust protection against brute-force attacks. The encryption function's complexity means that it would take years to crack a password that was encrypted using Bcrypt. The level of security it offers is unparalleled, and it is simple to implement.

How to Use Bcrypt with WordPress

Implementing Bcrypt into your WordPress password is relatively straightforward if you're comfortable making changes to your WordPress site's core files. You'll need to start by locating your WordPress's functions.php file, which can be accessed in your WordPress' Appearance > Editor.

Once you have located the functions.php file, you'll need to add the following code at the bottom of the file:

```php
function wpb_custom_passwords( $password ) {
  $salt = 'frthjt57kzgw89adw';
  return crypt( $password, '$2a$12$' . $salt );
}
add_filter( 'pre_user_pass', 'wpb_custom_passwords' );
```

This code creates a function wpb_custom_passwords that takes a user's password as an argument, generates a random salt value, combines it with the password to create an encrypted hash using Bcrypt, and returns the encrypted hash value.

Conclusion

The security of your WordPress password is crucial, and utilizing strong encryption methods such as Bcrypt can make it virtually impossible for hackers to crack passwords, even when using sophisticated software. Follow the steps outlined above to secure your WordPress account and stop hackers in their tracks. By using Bcrypt, you can take your online security seriously and protect yourself, your data, and your online reputation.

{{< youtube RtUvMJFP_IE >}} 



When we talk about password security, we often refer to the strength of your password and whether it can be easily guessed by hackers. However, one aspect of password security that few people talk about is how the password is stored in the database. In WordPress each password is usually salted and passed through MD5 hashing before it is stored in the database. It seems fine and secure until you find out that the MD5 algorithm is known to suffer from extensive vulnerabilities. According to CMU Software Engineering Institute, MD5 is essentially “cryptographically broken and unsuitable for further use.”
 
So what can you do to improve your WordPress password security? The answer is using bycrpt algorithm, particularly with the wp-password-bcrypt plugin.
 
bcrypt is based on the Blowfish cipher and is an adaptive function. This means that over time the iteration count can be increased to make it slower, so it remains resistant to brute-force search attacks even with increasing computation power.
 
Luckily, even if you are not technically competent, you can easily upgrade your WordPress system to replace MD5 hashing with the bcrypt algorithm.
 
1. Got to wp-password-bcrypt’s Github page and click the “Clone or download” button to download the ZIP file to your desktop.
 

 
2. Extract the zip file and open the extracted folder. All you need is the “wp-password-bcrypt.php” file.
 
3. With your FTP program (or cPanel) connect to your WordPress server and create a “mu-plugins” folder under the “wp-content” folder. This is also known as the “Must Use Plugins” folder, and all plugins placed in this folder are automatically activated. If the “mu-plugins” folder already exists, ignore this step.
 
4. Upload the “wp-password-bcrypt.php” file to this “mu-plugins” folder, and you are done.
 
What the “wp-password-bcrypt” plugin does is re-hash the password using bcrypt and store it in the database whenever a user logs in to the system. There is no configuration required, and everything simply works in the background. Do also note that if your site has a lot of inactive users who have not logged in for a long time, their passwords will still be using the MD5 hash.
 
Lastly, to uninstall the plugin, all you have to do is delete it from the “mu-plugins” folder. There are no negative consequences, and everything will continue to work as usual.
 
## Conclusion
 
It is completely useless for users to do everything they can to protect themselves if the system is insecure in the first place. By switching to using bcrypt algorithm, you can quickly and easily improve your WordPress password security and prevent your user account from being easily crackable (assuming they are using a strong password as well).
 
Image credit: Linux password file
 
Damien Oh started writing tech articles since 2007 and has over 10 years of experience in the tech industry. He is proficient in Windows, Linux, Mac, Android and iOS, and worked as a part time WordPress Developer. He is currently the owner and Editor-in-Chief of Make Tech Easier.
 
Our latest tutorials delivered straight to your inbox





---
title: "You'll Never Believe How Easy It Is to Protect Your Shared Windows PC with These Strong Password Tips!"
ShowToc: true 
date: "2023-04-07"
author: "Marjorie Crabtree"
---
*****
+++
title = "You'll Never Believe How Easy It Is to Protect Your Shared Windows PC with These Strong Password Tips!"
date = "2021-06-12"
author = "Anonymous"
tags = ["Windows PC", "password tips", "data protection"]
+++

If you're one of the many people using a shared Windows PC, you may be wondering how to keep your personal data safe from prying eyes. Luckily, protecting your Windows PC with a strong password is easier than you might think. Here are some simple tips to help you create a secure password and keep your personal data safe.

1. Use a longer password
One of the easiest ways to create a strong password is to use a longer one. The longer your password, the harder it is for someone to guess it. So, instead of using a 6-8-character password, aim for at least 12-16 characters or more. This will make it virtually impossible for someone to crack your password through brute force attacks.

2. Use a mix of uppercase and lowercase letters
Another way to create a strong password is to use a mix of uppercase and lowercase letters. Don't just stick to one case. Use a combination so that your password looks like a jumbled mess. This will make it harder for someone to guess your password by simply taking a guess based on your name or other easily identifiable information.

3. Use a mix of numbers and symbols
In addition to using a mix of uppercase and lowercase letters, you should also include numbers and symbols in your password. This will make it even harder for someone to guess your password. It is also recommended that you don't use commonly used symbols such as %, $, or #.

4. Avoid using easily guessable information
When creating a password, avoid using easily guessable information like your name, birthdate, favorite color, or pet name. These are the first things that hackers will try when attempting to crack your password. Instead, use an unguessable combination of letters, numbers, and symbols.

5. Use a password manager
If you find it difficult to remember all your different passwords, consider using a password manager. Password managers help you store all your passwords securely in one place, which means you only need to remember one master password. Password managers also make it easy to generate strong passwords and keep track of when you last changed your passwords.

In conclusion, creating a strong password is essential if you want to keep your personal data safe on a shared Windows PC. Follow these tips to create a strong password and ensure that your personal information is secure. Remember to also regularly update your password and avoid sharing it with others. By taking these simple steps, you can protect your data and enjoy peace of mind knowing that your Windows PC is safe from unauthorized access.

{{< youtube Fg03d5A-0gY >}} 



Creating a strong and complex password is one of the best ways to protect your account and your PC from any type of compromise or other security threat. You can certainly make sure that your own password is hard to crack, but how can you coax other people who use the same PC to do likewise?
Large companies and enterprises typically set up domains and rely on Group Policy to set password policies. But your average home or even small office isn't likely to go through the trouble of creating and managing domains. No problem. You can still protect your shared computer by using the local security policy in Windows. Available in Windows 10 and 11, the local security policy helps you control a variety of security options for all users of the PC, including password length and complexity.
Many of the settings offered by the local security policy are geared toward domain-based computers. But if you simply want to control a single computer, you can ignore the network-specific settings and focus on the ones for passwords. Using the policy this way will help you better protect a PC shared in a home, a home office, or a small business office. Let's see how this works.

 
## How to set local security policy in Windows


The local security policy is accessible from Windows 10 and 11 and works the same in both versions. You can open or access the local security policy using a few different methods. But the quickest way is through the Search tool. Click the Search field or icon, type secpol.msc, and then press Enter. The local security policy window pops up (Figure 1).

 
## Set minimum password length


First, you can ensure that anyone who has an account on this computer uses a password of a certain length. Click the right arrow for Account Policies and then select Password Policy. Among the eight options here, double-click the one for Minimum Password Length.
Click the Explain tab to see the details of this setting. By default, the minimum length can be as many as 14 characters. Switch back to the Local Security Setting Tab and enter a number up to 14 to specify the minimum length for a password. Click OK when done (Figure 2).

 
## Set password complexity


More important than password length is complexity, which means requiring users of this shared PC to use passwords with uppercase and lowercase characters, numbers, and non-alphanumeric characters. Double-click the option for Password must meet complexity requirements.
Click the Explain tab to see the requirements for this one. If this policy is enabled, the password can't contain the user's account name and must be at least six characters long. It also must contain characters from any three of the following categories: Uppercase characters, lowercase characters, any number 0 through 9, and non-alphanumeric characters such as ! or #. Go back to the Local Security Setting tab and click the button for Enabled. Click OK (Figure 3).

 
## Require password changes


Next, you can make sure that people must change their passwords periodically. Double-click the option for Maximum Password Age. Select  the Explain tab to learn how this setting works. Return to the Local  Security Setting tab and enter a number to determine how many days  someone can use a password before it expires. Depending on your  environment, 90 days is typically a good timeframe, so that people have  to change their passwords every three months. Click OK (Figure 4).  

 
## Enforce password history


Faced with the challenge of changing their passwords periodically, many people will simply recycle older passwords. You can limit this tendency by enforcing a password history. Click the option for Enforce password history. Click the Explain tab to see how this plays out. At the Local Security Setting screen, enter a number between 0 and 24, with 0 meaning that no password will be remembered and 24 meaning that the past two dozen passwords will be remembered and therefore unable to be reused. Click OK (Figure 5).

 
## Set lockout policy


Next, you can protect your PC's accounts from compromise by locking them out if the wrong password is entered too many times. Select the setting for Account Lockout Policy and double-click the option for Account lockout threshold.
Click the Explain tab to read the details on this one. Return to the Local Security Setting screen and enter a number between 0 and 999. The number will determine how many times an incorrect password can be entered before the account is locked out. A locked out account then must be reset by an administrator account on that PC. Click OK.
Based on the number you choose, you may see suggestions for the other two options: Account lockout duration and Reset account lockout counter. These two options determine how long the account will be locked out following the specified number of wrong password attempts. Click OK to accept the suggested settings (Figure 6).
How strict should you make the password and lockout requirements on your shared PC? That depends on the location and the people using it. For a home PC used by family members, you may want to keep the settings less restrictive. But for a business PC used by employees, you might tighten the requirements. Of course, you can always adjust the settings if they turn out to be too loose or too tight.






---
title: "Are You Making These Jquery Mistakes? Learn How To Safely and Wisely Use It!"
ShowToc: true 
date: "2023-01-13"
author: "Luis Tiefenauer"
---
*****
Are You Making These Jquery Mistakes? Learn How To Safely and Wisely Use It!

In the world of web development, jQuery is a well-known JavaScript library that makes coding easier and more efficient. However, its popularity has made it prone to misuse and have led to certain errors and misconceptions.

If you're new to jQuery, tread carefully and learn how to use it wisely to avoid these common mistakes:

Not Using the Latest Version

Like most software, jQuery goes through updates for optimization and security fixes. Some developers, however, tend to stick to older versions and miss out on new features that can make their code more efficient.

Keep up with the latest version of jQuery, and evaluate any changes that could benefit your code. This way, you avoid using outdated features and improve the functionality of your website.

Overusing jQuery Selectors

JQuery offers a vast array of selectors that allow developers to easily target HTML elements. However, using too many selectors can cause performance issues and slow down page loading times.

Instead of using many selectors, be selective in which elements you target. Focus on specific elements that need modifications, and try to avoid unnecessary HTML tags.

Not Optimizing Code

One of the most common mistakes in web development is not optimizing code. With jQuery, you can avoid this by careful structuring and organization of your code.

One common technique is to use chained functions, which allows you to streamline your code and make it more readable. Another technique is to minimize the use of repetitive code by creating reusable functions.

Not Using jQuery's Built-in Functions

jQuery offers several built-in functions that can help automate repetitive tasks, such as animations and event handling. However, some developers tend to use native JavaScript methods instead of jQuery's built-in functions.

Using jQuery's built-in functions saves time and code by simplifying complex tasks. These functions were designed to handle cross-browser compatibility and offer a standardized process for handling events and animations.

Not Understanding the DOM

One of the most basic pitfalls of jQuery is not understanding how it interacts with the DOM (Document Object Model). Understanding the basics of the DOM can help you better utilize jQuery to manipulate elements and CSS styles.

The DOM is a hierarchical structure that represents the HTML layout of your website. When using jQuery, it's important to understand how elements are structured and how they can be manipulated with the library.

In summary, using jQuery is beneficial for web development, but it must be done wisely. Avoid these common mistakes by keeping up with the latest version, being selective with selectors, optimizing code, using jQuery's built-in functions, and understanding the DOM. When used properly, jQuery can enhance web development and make coding more efficient.

{{< youtube sF0q6t1Q_Xc >}} 



Now we can begin.
Quick introduction to jQuery 
A lot of times, as developers work daily on new versions of web pages, you’ll hear them say, “Good God, I thank you for giving me jQuery.”
What is jQuery? It is a lightweight programming library for JavaScript. Its main task is to manipulate the DOM tree of elements. What does it really offer? Now, in exchange for a really small performance decrease compared to a professionally written code in JavaScript, we get the opportunity to achieve amazing animation effects on our website. In addition, we can also make dynamic changes and do all of the Ajax requests. In fact, most of the available jQuery plugins do not require any changes to the HTML source. Ok, that should be enough introduction. Let’s move on.
Reasonable use of jQuery on () Event to prevent default user shares
This problem is really very interesting. Wcielmy is a bad hacker. What happens if he can invoke the default action using jQuery? Can it therefore call any action on your website? Or maybe he can do something more? So, the jQuery creator gave us something extra as developers. And that is a function of a (), which we can use to prevent the default action of the user when the user clicks on the link. Previously, we were using one of the default values by clicking on the redirect link. These were the “#”, “javascript :/ /”, “javascript.void (0)”. Today, however, we are dealing with something a little different. Namely, we can capture all the events using event.preventDefault (), which is called in the middle of a function. This is perfectly illustrated in the code below:
/ / Be careful what parameters you give to the function on ()
/ / Note that we do the event within the function ()
$ (“# Something”). On (“click”, “a”, function (event) {
event.preventDefault () / / preventDefault ()
/ / Now we can do something
/ / It’s also advised to be careful and do not leave it on so the
});
Note that the structure of the jQuery library has a lot of technical reasons why jQuery uses these options on the function (). To know more about the features on (), you can, of course, read the documentation for the jQuery library. Here is the link: http://api.jquery.com/on/.
Threats coming from Reply () 
This error is not really strictly from jQuery. After jQuery, everything related to JavaScript is running on the client side. So how does using Reply () become dangerous? Consider the specific case. If you’re using Reply and download data for a logged in user, you might have a problem. As an attacker, I can look into the code and see there the following. Now, notice that pass user id probably used in jQuery. It is enough that with a slight modifying of your script, I can type a different user id.
But what if you want to hide anything? And when I use validation? Well, of course they are not bad habits, but I would not only rely on jQuery or JavaScript. In addition, I’d be sure to check again that everything on the server side is certainly OK. Really, this is particularly important when you start thinking about using Ajax and DOM tree elements. In addition, I would always be 100% sure whether it will work even when JavaScript is disabled.
Again, notice what I wrote. Well, if you do not make server-side filtering relevant nor check permissions of your users, or if you do not check if we can perform a code injection, everything is invalid and this will not help you. Every time I would be able to manipulate your data as much as I want, and it will not really cost you too much work. But also note one more thing. Even when you are not using jQuery, if your template is a form POST, I can also do it. How do you use GET? My action is simpler; I just type your address with the appropriate parameters. So as you can see, this solution is not really related to jQuery, but with skills in programming.
Errors in the old versions 
I’ll say this: oh, God. Why use an old version of jQuery? What are you really after? Note that in the case of web applications and the languages used in their construction, each new version gives a lot of great improvements. First, the new version will always include amendments that affect safety and performance. Tell me, what is the point of using the old version of jQuery for new projects?
Do you know how many bugs can appear on a jQuery project? Check it out and see if it is related to security issues. Using the old version is justified, but only in one case only. Well, sometimes the customer may require the use of an outdated version. If the customer is paying for it, you should be sure to do so. But if you have an old project with an old version of jQuery, do not hesitate, just go ahead and change it to a newer version. Removal of errors that may occur will certainly be cheaper to implement than using outdated versions. The website has to load fast. What do I care if it has great visual effects if it takes an hour to load?
JQuery storage of the root page template 
Another fundamental error: If an attacker knows how to get to the subject, he is able to make many changes to multiple files. It can also replace the local version of jQuery with its own. And then what? The whole can begin to act as the attacker wants. Really it can then be interesting. And how do we fix it for a client? The customer can take offense at us and will never take advantage of our services. This also shows one more very important thing. Well, it is better to take advantage of the global copy of the jQuery library, contained for example in a Google API. This solution also has a substantial advantage. Using jQuery from an external server, namely the Google API, allows the search engine to continuously monitor our site. Not only do we have access to all of Google’s information, such as the number of visitors, it’s also in the event of any problems with our site, Google will inform you about the infected site. We can even put the link:
<script src=”//ajax.googleapis.com/ajax/libs/jquery/1.8.0/jquery.min.js” <script type=”text/javascript”></ script>
Always check each jQuery plugin before you throw it on your site 
Man, after all, jQuery is not that hard. Before you throw something on your site, I always see this code. Do not let even the best plugin which does great things with the graphics on your website cause a failure. Do not allow this to happen, or you would not know what exactly is happening on your website.
As I mentioned, understanding jQuery is not difficult. But what in case if you write your own code? Then writing a good jQuery script can be terribly difficult. You must unfortunately rely on trial and error. And then what? Do you have to rely on trial and error to find out what is good and what is not? Does it have to be this way? Of course not.
If you create your own design, you can easily reduce the risk by following some very simple tests. If you write a jQuery script, also be a quality engineer. Start by checking the size of the file that contains your jQuery script. If the value is greater than the base library, there really is something wrong. Then, recall the article which describes Firebug. Firebug allows you to quickly and easily find a place where something is wrong. Firebug also allows you to check if indeed everything is in place and is behaving as it should.
In addition, it is necessary to test the site on all possible browsers, and do not forget that today everything is mobile. Really make sure that the plugin runs on the phone and was not the cause of the crash. Check it out on iOS, check it out for Android, and check it on Windows Mobile. The rest is irrelevant today.
Please, go to OWASP 
This is another very important thing for you. Here you will find information on possible attacks on websites. Read the top 10 list on how you can manipulate the script and attach to their data, and particularly check that all the information is in order to manipulate the scripts, JavaScript, and DOM tree elements. Reviewing this may prevent you from making mistakes in the future. It is really important if you want to create secure applications.
Everything you write, test 
You must test each function in jQuery you write. Select the limits for it, the max and min, and then do max +1, min +1. If the function to display images is in any order, make sure it is really safe. Test the function of equipment, if you have any arguments, so pointless arguments scratch those that just come up. This is the process of software testing. Do it when you write a script or plugin, and by the way you will save yourself a lot of time later. If you do, you can be sure that your application is sure to be safe, but it does not mean it would be vulnerable to external manipulation.
Bug Tracker 
Be sure to see bug tracker for jQuery. Be sure to click on this link http://bugs.jquery.com/newticket? redirectedfrom to see a list of bugs. There’s no point in leaving anything to chance. Also check the disadvantages of each version of jQuery you are using, and then see how it solved the problem. See if the same problem then occurs in other versions. This is extremely important. Sometimes using some version of jQuery could mess up something good on your computer. Remember that jQuery is a library of programming, based on JavaScript. That’s what you do with JavaScript, but faster and more efficiently done using jQuery. View this page http://bugs.jquery.com/timeline and see what the errors in jQuery are. Learn how to write scripts, as well as how to throw them onto the page. Always know what script or plugin loaded on your site and know what it is really doing.
Summary 
This article shows not just the weakness of jQuery, but also how to write well and post jQuery scripts. It is actually the most common source of errors in this type of application: poorly written scripts, the scripts downloaded nowhere, a lack of knowledge on which the basis of the script works.
Remember again that jQuery does not work on the server side. It works as JavaScript, on the user side, or on the side of the search engine. If you are not sure if it is worth exposing, turn off jQuery, Ajax and JavaScript. It’s your choice. Properly used, jQuery is not dangerous, but jQuery already used otherwise can be very dangerous.
If you want me to show you how you can cleverly manipulate using jQuery and Ajax, just write to me. Or write to Rob and he would let me know if you want to. Believe me – you can really do more here than that if it was on the server side.






---
title: "Revolutionize Your Workflow Now: Here's the Secret to Installing Google Assistant on Windows 10!"
ShowToc: true 
date: "2023-01-04"
author: "Raymond Wagner"
---
*****
Revolutionize Your Workflow Now: Here's the Secret to Installing Google Assistant on Windows 10!

If you've ever wished that you could have a personal assistant to help you with your daily tasks, then you're in luck. Google Assistant is an artificial intelligence-powered virtual assistant that can help you do just that. And with the recent developments in the world of technology, it is now possible to install Google Assistant on your Windows 10 operating system. In this article, we're going to show you how to revolutionize your workflow by installing Google Assistant on your Windows 10 computer.

The Benefits of Google Assistant

For those who are unfamiliar with Google Assistant, here are some of the benefits of using it:

1. Convenience: Google Assistant is designed to simplify your life by handling various tasks for you, such as setting up reminders, playing music, and making phone calls. You can use your voice to interact with Google Assistant, which makes it more convenient than typing or clicking.

2. Customization: Google Assistant can be customized to suit your needs. You can set up routines that automate certain tasks, such as turning off your lights when you leave for work, or turning on your coffee maker in the morning.

3. Accessibility: Google Assistant is compatible with various devices, including smartphones, smart speakers, and even cars. This means that you can access it wherever you are, and whatever you're doing.

How to Install Google Assistant on Windows 10

Now that you know why Google Assistant is such an essential tool for your workflow, let's dive into the steps for installing it on your Windows 10 computer:

Step 1: Download and Install Python

The first step in the installation process involves downloading and installing Python, which is a programming language that Google Assistant requires to run. Here's how to do it:

1. Go to the Python website and download the latest version of Python for Windows.

2. Open the downloaded file and follow the installation wizard.

3. During the installation process, make sure to check the "Add Python to PATH" option, which will enable you to run Python from the command line.

Step 2: Install Google Assistant

Once you've installed Python, you'll need to install Google Assistant. Here are the steps:

1. Open the command prompt by pressing the Windows key + R, typing "cmd" in the search box, and hitting Enter.

2. Type the following command in the command prompt:

pip install google-assistant-sdk[samples]

3. This command will download and install the Google Assistant SDK, along with some sample code that you can use to test it.

Step 3: Set Up a Google Project and Configure Google Assistant

Now that you have installed Google Assistant, the next step is to set up a Google project and configure it. Here's how to do it:

1. Go to the Google Cloud Console website and create a new project.

2. Once you've created a project, go to the credentials tab and create a new OAuth client ID.

3. Select "Windows" as the application type, enter a name for your client ID, and click "Create."

4. On the next screen, download the client ID JSON file.

5. Place the JSON file in a directory on your computer.

6. In the command prompt, type the following command:

python -m googlesamples.assistant.auth_helpers --client-secrets "path_to_client_secrets.json"

7. This command will prompt you to log in to your Google account and authorize the Google Assistant API.

8. Finally, run the following command to start Google Assistant:

python -m googlesamples.assistant --project-id PROJECT_ID --device-model-id DEVICE_MODEL_ID

Congratulations! You have successfully installed Google Assistant on your Windows 10 computer.

Conclusion

By installing Google Assistant on your Windows 10 computer, you can revolutionize your workflow and increase your productivity. With its voice-activated interface and customizable features, Google Assistant can help you simplify your life and automate your daily tasks. Follow the steps outlined in this article, and you'll be on your way to enjoying the benefits of Google Assistant on your Windows 10 computer.

{{< youtube -feDcvdeVpY >}} 




 
To get Google Assistant on PC, you need to follow command-line instructions, which is the only way to get it on PC. Anyway, without wasting any time, let’s see How to Get Google Assistant on Windows 10 with the below-listed guide’s help.
 
## How to Install Google Assistant on Windows 10
 
Make sure to create a restore point just in case something goes wrong.
 
Contents
 
- How to Install Google Assistant on Windows 10
 - Prerequisites:
 - Step 1: Configure the Google Assistant API
 - Step 2: Install Google Assistant Sample Python Project
 - Step 3: Testing Google Assistant on Windows 10 PC

 
#### Prerequisites:
 
1. First, you need to download Python on your PC.
 
2. Download Python 3.6.4 from the link, then double-click on python-3.6.4.exe to run the setup.
 
3. Checkmark “Add Python 3.6 to PATH,” then click on Customize installation.
 
4. Make sure everything is checked in the window, then click Next.
 
5. On the next screen, just make sure to checkmark “Add Python to environment variables.”
 
6. Click Install, then wait for Python to get installed on your PC.
 
7. Once the installation is complete, restart your PC.
 
8. Now, press Windows Key + X, then select Command Prompt (Admin).
 
9. Type the following command into cmd and hit Enter:
 
python
 
10. If the above command will return the current Python version on your computer, then you have successfully installed Python NumPy on your PC.
 
#### Step 1: Configure the Google Assistant API
 
With this step, you can use Google Assistant on Windows, Mac, or Linux. Just install the python on each of these OS to properly configure Google Assistant API.
 
1. First, go to the Google Cloud Platform Console website and click on CREATE PROJECT. 
 
Note: You might need to sign in with your Google account.
 
2. Name your project appropriately, then click on Create.
 
Note: Make sure to note down the project ID, in our case, its windows10-201802. 
 
3. Wait till your new project is created (you will notice a spinning circle on the bell icon at the top right corner).
 
4. Once the process is done click on the bell icon and select your project.
 
5. On the project page, from the left-hand menu, click on APIs & Services, then select Library.
 
6. On the library page, search for “Google Assistant” (without quotes) in the search console.
 
7. Click on Google Assistant API search result and then click on Enable.
 
8. Now, from the left-hand menu, click on Credentials, then click “Create credentials” and then select Help me choose.
 
9. Choose the following information on the “Add credentials to your project” screen:
 
Question: Which API are you using? 

Answer: Google Assistant API



Question: Where will you be calling the API form?

Answer: Other UI (e.g. Windows, CLI tool)



Question: What data will you be accessing?

Answer: User data
 
10. After answering all of the above questions, click on “What credentials do I need?“.
 
11. Select Set up consent screen and choose the Application type to Internal. Type the project name in the Application name and click Save.
 
12. Again, go back to the “Add credentials to your project” screen, then click on Create Credentials and select Help me choose. Follow the same instructions as you did on step 9 and proceed forward.
 
13. Next, type the name of the Client ID (name it anything you like) to create OAuth 2.0 client ID and click on the Create Client ID button.
 
14. Click Done, then open a new tab and go to Activity controls from this link.
 
15. Make sure all the toggles are turned ON and then go back to the Credentials tab.
 
16. Click the download icon in the far right of the screen to download the credentials.
 
Note: Save the credentials file somewhere easily accessible.
 
#### Step 2: Install Google Assistant Sample Python Project
 
1. Press Windows Key + X then select Command Prompt (Admin).
 
2. Type the following command into cmd and hit Enter after each one:
 
py -m pip install google-assistant-sdk[samples]
 
3. Once the above command finishes executing, type the below command and hit Enter.
 
pip install --upgrade google-auth-oauthlib[tool]


 
4. Navigate to the JSON file location that you downloaded earlier and right-click on it and select Properties. In the name field, copy the file name and paste it inside notepad.
 
5. Now enter the below command but make sure to replace the “path/to/client_secret_XXXXX.json” with the actual path of your JSON file which you copied above:
 
google-oauthlib-tool --client-secrets path/to/client_secret_XXXXX.json --scope https://www.googleapis.com/auth/assistant-sdk-prototype --save --headless
 
6. Once the above command finishes processing, you get a URL as the output. Make sure to copy this URL as you will require it in the next step. 
 
Note: Don’t close the Command Prompt just yet.
 
7. Open your Web browser and navigate to this URL, then select the same Google account that you used to configure the Google Assistant API.
 
8. Make sure to click on Allow to grant the necessary permission to run Google Assitant.
 
9. On the next page, you will see some code that will be your client’s Access Token.
 
10. Now switch back to the Command prompt and copy this code & paste it into cmd. If everything goes alright you see an output that says that your credentials have been saved.
 
#### Step 3: Testing Google Assistant on Windows 10 PC
 
2. Now we need to test if Google Assistant can properly access your microphone. Type the below command into cmd and hit Enter, which will start a 5-second audio recording:
 
py -m googlesamples.assistant.grpc.audio_helpers
 
3. If you can successfully hear the 5-second audio recording back, you can move to the next step.
 
Note: You can also use the below command as an alternative:
 
googlesamples-assistant-audiotest --record-time 10
 
4. You need to Register your Device before you can start using Google Assistant on Windows 10 PC.
 
5. Next, type the below command and press Enter:
 
cd C:\GoogleAssistant
 
6. Now type the following command but replace the “project-id” with the actual project id that you have created in the first step. In our case it was windows10-201802.
 
googlesamples-assistant-devicetool --project-id register-model --manufacturer "Assistant SDK developer" --product-name "Assistant SDK light" --type LIGHT --model "GA4W"
 
7. Next, to enable Google Assistant Push to Talk (PTT) capabilities, enter the below command below but make sure to replace “project-id” with the actual project id:
 
py -m googlesamples.assistant.grpc.pushtotalk --device-model-id “GA4W” --project-id
 
Note: The Google Assistant API supports every command that Google Assistant supports on Android and Google Home.
 
You have successfully installed & configured Google Assistant on your Windows 10 PC. Once you enter the above command, simply press Enter and you can ask any questions directly to Google Assistant without having to say “OK, Google” command.
 
Recommended:
 
- Completely uninstall Norton from Windows 10
 - How to Setup Remote Desktop Connection on Windows 10
 - Automatically disable Touchpad when Mouse is connected
 - How to completely uninstall McAfee from Windows 10

 
We hope this guide was helpful and you were able to install Google Assistant on Windows 10 PC without any issues. But if you still have any questions regarding this guide, then feel free to ask them in the comment section.





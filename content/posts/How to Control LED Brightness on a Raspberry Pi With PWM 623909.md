---
title: "Unlock the Secrets of LED Control on Raspberry Pi with this Simple PWM Trick!"
ShowToc: true 
date: "2023-03-28"
author: "Kim Romney"
---
*****
Title: Unlock the Secrets of LED Control on Raspberry Pi with this Simple PWM Trick!

Introduction:

Are you an avid Raspberry Pi user who is looking to delve deeper into LED control? If so, then you’ve come to the right place! In this article, we’ll be exploring the basics of Pulse Width Modulation (PWM) and how you can use it to control your LEDs on Raspberry Pi.

What is PWM?

Pulse Width Modulation (PWM) is a technique used to control the amount of power delivered to electronic devices, such as LEDs. By rapidly switching a signal “on” and “off”, PWM can effectively control the amount of current flowing through a device, resulting in a varying amount of brightness or intensity.

The traditional method of controlling an LED on Raspberry Pi involves turning it “on” or “off” through a simple circuit. However, this method can be limiting as it can only provide a fixed level of illumination. PWM, on the other hand, offers much more control, allowing you to adjust the intensity of your LED’s light output.

How to Use PWM on Raspberry Pi:

To begin, you’ll need to import the GPIO library (General Purpose Input/Output) into your Raspberry Pi project. Once you’ve done this, you can create a PWM object by specifying the pin number and the frequency, in hertz.

Here’s an example code snippet to get you started:

```python
import RPi.GPIO as GPIO
from time import sleep

GPIO.setmode(GPIO.BOARD)

led_pin = 11
GPIO.setup(led_pin, GPIO.OUT)

pwm_led = GPIO.PWM(led_pin, 200)
pwm_led.start(0)

while True:
    for duty_cycle in range(0, 101, 5):
        pwm_led.ChangeDutyCycle(duty_cycle)
        sleep(0.1)
```

In this example, we’ve set up a PWM object on pin 11 with a frequency of 200 hertz. The ```pwm_led.start(0)``` line is used to initialize the PWM with a duty cycle of 0%, effectively turning off the LED at the start of the program.

The ```while True``` loop cycles through a range of duty cycles from 0 to 100, in increments of 5. The ```ChangeDutyCycle()``` method is used to adjust the duty cycle of the PWM object during each iteration of the loop, resulting in a smooth transition from low to high LED intensity.

Conclusion:

In conclusion, PWM is a powerful technique that can be used to control the intensity of LEDs on Raspberry Pi. By using a simple code snippet like the one above, you can experiment with different frequencies and duty cycles to achieve the perfect lighting effect for your project.

Whether you’re a hobbyist, student or professional, there are endless possibilities when it comes to creating LED-based projects on Raspberry Pi. So what are you waiting for? Go ahead and unlock the secrets of LED control with PWM and take your project to the next level!

{{< youtube RA06ee3jahM >}} 



If you had fun making LEDs blink on a Raspberry Pi, wait until you hear about controlling its brightness! In this guide, we work with a pair of buttons to adjust the led brightness on a Raspberry Pi.
 
Starting your first Raspberry Pi project? Here’s how to quickly install Raspberry Pi OS on your device. 
 
## What PWM Does to an LED
 
PWM, or Pulse Width Modulation, is a method that artificially lowers the voltage output of the Raspberry Pi’s GPIO (General Purpose Input/Output) pins. It’s artificial, as you don’t really reduce the voltage and just turn it on and off so fast that the overall voltage becomes lower than the real voltage you’re applying to it.
 
For an LED or Light-Emitting Diode, increasing the overall voltage makes it shine brighter, while decreasing it makes it dimmer. But since the Raspberry Pi has no analog output, we’re using PWM to control the LED’s brightness.
 
## What You’ll Need
 
- 2 pushbuttons
 - 3 resistors (250-550Ω will work. Use a lower rating if the LED is too dark.)
 - 1 LED (any color)
 - Breadboard
 - Jumper wires
 - Raspberry Pi (any model except the Pi Pico)

 
## How to Use PWM to Control LED Brightness on a Raspberry Pi
 
In this guide, we are using use two buttons to make the LED shine brighter or dimmer with PWM. Pressing the “brighter” button increases the PWM output, while pressing the “dimmer” button decreases it.
 
### Preparing the Circuit
 
- Let’s start with the LED. On the breadboard, place the LED and connect a resistor to one side. The side the resistor is placed does not matter.

 
- Connect a jumper to its cathode side. This one will point to pin 11 on the Raspberry Pi. Add another jumper that leads to the blue rail on the breadboard, then add another jumper from that blue rail to pin 9 on the Raspberry Pi, which is GND.

 
Note: to find the right pin number on the Raspberry Pi, hold the board so that the GPIO pin tray sits to the right. The top-left pin should be pin 1, to its right should be pin 2, and below should be pin 3.
 
- You’ll need to build the pushbuttons. Place the pushbuttons on the breadboard and add a resistor to one leg of each pushbutton. The other side of the resistor should lead to the blue rail of the breadboard.

 
Tip: want to know more about pushbuttons? We have a full guide dedicated to showing you how to use pushbuttons with Raspberry Pi GPIO pins.
 
- Add jumper wires in a parallel connection with the resistor and pushbutton. Connect the other side of these to pins 13 (“Brighter” button) and 15 (“Dimmer” button).

 
- Use a jumper wire to connect the pushbuttons to the side with the red rail of the breadboard.

 
- Connect the red rail to a 3.3V source on the Raspberry Pi, like pin 1.

 
If Python is your go-to programming language, learn how to install and manage multiple Python versions in Linux. 
 
### Preparing the Code
 
On your favorite code-editing tool, make a new file and save it as “rpi-lcdpwm.py.”
 
- Start with the code below, which gives you two ways of importing modules on Python: the first imports the RPi.GPIO module and lets you call it with just GPIO, and the second one imports only the sleep() function from the entirety of the time module.

 
- Define the pin numbers to make it easier to change pins in case you change your mind later on.

 
- Optional: add the line GPIO.setwarnings(False) so that you can avoid the GPIO warning message when you start the script later.

 
- Set the pin selection method. BOARD is a good choice for beginners, as it makes it easier to look for pins without having to consult the pinout. The other method is BCM, which stands for “Broadcom.” This uses the Broadcom numbers assigned to each pin, which may differ based on your Raspberry Pi’s make.

 
- Assign the GPIO pins as input or output. We’re assigning ledPin as an output pin and will always start its state as LOW. The next two lines set brightenButton and dimButton as input pins that listen to your button pushes. These should also be set as GPIO.PUD_DOWN to designate them as using pulldown resistors.

 
- Let’s declare the PWM. pwmLEDPin is a variable that makes it easier to type GPIO.PWM(ledPin, 100) later on, and the .start(0) command begins the PWM process. We can now change the output of ledPin using PWM.

 
- The duty cycle is the percentage of time that the pin is active during a pulse wave. Here, we’re setting the duty cycle to 100% first. We had a rather lengthy discussion on this topic in our guide to using servo motors with the Raspberry Pi, if you’re interested.

 
- For the looping part, we are setting a while loop that runs virtually forever.

 
- At the beginning of this looping cycle, we are updating the duty cycle.

 
- Let’s program what the brightenButton does. When the Raspberry detects electricity passing through the pin for brightenButton, it will show a message that says “brightenButton is HIGH,” which adds 5 to the current value of the duty cycle until it reaches 100.

 
- When programming the dimButton function, it does the opposite, reducing the value by 5 until it reaches 0.

 
### Final Code:
 
## Making It Work
 
First, you’ll need a terminal. You can use the Raspberry Pi’s built-in terminal or control the Raspberry Pi through SSH on a separate computer. Through the terminal, you should go to the Python script’s directory and enter python3 rpi-ledpwm.py or the filename you used.
 
Sometimes the LED will look like it’s blinking. The PWM frequency is probably too low, if that’s the case. You can increase the frequency by increasing the number in pwmLEDPin = GPIO.PWM(ledPin, 100) until the blinking is no longer noticeable.
 
If you find the transitions to be grainy, lower the time in sleep(0.25) inside the while loop. It does get faster as you lower it, though, so don’t lower it too much.
 
Tip: prefer Arduino instead? Here’s a complete guide to getting you started with Arduino projects. 
 
## Frequently Asked Questions
 
All images by Terenz Jomar Dela Cruz.
 
### What is the minimum frequency I can generate with the Raspberry Pi?
 
The lowest frequency you can set on a Raspberry Pi is 10Hz. The hardware can’t support anything lower than that.
 
### What is the maximum frequency I can generate with the Raspberry Pi?
 
The highest frequency you can set on a Raspberry Pi is 8,000Hz.
 
### Is it possible to turn pulse waves into sound waves?
 
Yes. With a piezoelectric element, it is entirely possible to turn pulse waves into sound waves that you can hear. In this case, modifying the frequency changes the pitch, while modifying the duty cycle adjusts the volume.
 
Terenz is a hobbyist roboticist trying to build the most awesome robot the world has ever seen. He could have done that already if he wasn't so busy burning through LEDs as a second hobby.
 
Our latest tutorials delivered straight to your inbox





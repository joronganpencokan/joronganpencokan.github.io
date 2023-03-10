---
title: "Unleash the Power of Raspberry Pi: Learn How to Create Mesmerizing Blinking LEDs!"
ShowToc: true 
date: "2023-06-23"
author: "Margaret Brumfield"
---
*****
# Unleash the Power of Raspberry Pi: Learn How to Create Mesmerizing Blinking LEDs!

Are you a tech enthusiast who loves to explore new gadgets and experiment with them? If so, you may have heard of the Raspberry Pi, a tiny yet powerful computer that's widely used in DIY projects and as a learning tool for coding and electronics.

One of the coolest things you can do with a Raspberry Pi is to create mesmerizing blinking LEDs. This may sound like a simple task, but the possibilities are endless, and the results can be stunning.

In this tutorial, you'll learn how to unleash the power of Raspberry Pi and create your own LED light show. Here are the steps:

## Step 1: Get the Materials

First, you'll need to gather the necessary materials. Here's a list of what you'll need:

- Raspberry Pi (any model will do)
- Breadboard
- LED lights (any color)
- Jumper wires (male-to-male and male-to-female)
- Resistors (220 ohms)
- Power supply (5V, 2A)

You can buy these components online or from a local electronics store. They're relatively inexpensive and widely available.

## Step 2: Connect the Components

Next, you'll need to connect the components to create a circuit. Follow these steps:

1. Place the Raspberry Pi on a flat surface, and connect it to the power supply using a micro-USB cable.

2. Insert the male-to-female jumper wires into the breadboard, as shown in the picture below. The wires should be aligned vertically, with one row for each LED.

3. Connect the 220-ohm resistors to the longer leg of each LED. The resistors will limit the current flowing through the LEDs, preventing them from burning out.

4. Connect the other end of each resistor to a jumper wire on the breadboard. You should have one wire for each LED.

5. Connect the male-to-male jumper wires from the Raspberry Pi to the breadboard, as shown in the picture below. You'll need to connect them to the GPIO pins, which are the small pins on the edge of the Raspberry Pi.

6. Finally, connect the female end of each jumper wire to the corresponding wire on the breadboard. Make sure the colors match, so you don't get confused later.

Congratulations! You've created a circuit that can control multiple LEDs using a Raspberry Pi.

## Step 3: Program the Raspberry Pi

Now comes the fun part: programming the Raspberry Pi to control the LEDs. There are different programming languages you can use for this task, but we'll use Python, which is beginner-friendly and powerful enough to handle complex projects.

1. Open the Terminal on your Raspberry Pi, and type the following command to install the RPi.GPIO library, which will allow us to control the GPIO pins:

```bash
sudo apt-get update
sudo apt-get install rpi.gpio
```

2. Create a new Python file using your favorite text editor or IDE. You can name it anything you like, but make sure it has a `.py` extension, such as `leds.py`.

3. Copy and paste the following code into your Python file:

```python
import RPi.GPIO as GPIO
import time

GPIO.setmode(GPIO.BCM)

led_pins = [18, 23, 24] # Change these to match your circuit
delay = 0.5 # Change this to adjust the blinking speed

for pin in led_pins:
    GPIO.setup(pin, GPIO.OUT)

try:
    while True:
        for i in range(len(led_pins)):
            GPIO.output(led_pins[i], GPIO.HIGH)
            time.sleep(delay)
            GPIO.output(led_pins[i], GPIO.LOW)
except KeyboardInterrupt:
    GPIO.cleanup()
```

4. Save your Python file, and run it from the Terminal using the following command:

```bash
python3 leds.py
```

If everything goes well, you should see your LED lights start blinking in a mesmerizing pattern. You can modify the code to create different patterns or add more LEDs to the circuit.

## Conclusion

By following these simple steps, you've learned how to unleash the power of Raspberry Pi and create mesmerizing blinking LEDs. This is just the tip of the iceberg, as there are countless other projects you can do with a Raspberry Pi, from controlling robots to building smart homes.

If you're new to coding and electronics, this project can be a great starting point for your journey. And if you're already an experienced maker, you can use this project as a building block for more advanced projects. Either way, have fun, and let your imagination soar!

{{< youtube 7YLF-N0596I >}} 



The Raspberry Pi is more than just a tiny computer. It’s a powerful board that lets you do so many things with its GPIO pins. Here we show you how to make blinking LEDs with the Raspberry Pi.
 
## What Makes the LEDs Blink?
 
When you look at the top part of your Raspberry Pi, you’ll find about 40 metal pins jutting out of the circuit board. If you have a Raspberry Zero, there is probably circular holes for soldering header pins. In either case, they are called GPIO pins (General Purpose Input / Output).
 
Each GPIO pin is made to have one of two modes at any given time: a HIGH and a LOW. For the Raspberry Pi’s pinout specifications, a pin charged at 3.3 V counts as a HIGH or a “logical 1,” while anything below around 2.5-ish V counts as a LOW or “logical 0.” A board that’s based on 3.3 V for high and low outputs is said to be on “3.3v logic.”
 
When you connect an LED between a pin on HIGH and a GND pin, you’re basically making a complete circuit. The LED should light up because of the passing electricity.
 
Sometimes your LEDs will pop in smoke when there’s too much current passing through it. To keep that from happening, you can add a resistor. It doesn’t matter whether it’s on the anode or cathode side – either side should decrease the current passing through.
 
### GPIO and Other Pins
 
Let’s be clear here, as not all of those metal pins are considered GPIO. They are only GPIO if they can be programmed to have a high or low – hence the term “Input / Output.” For the Raspberry PI, there are also pins made for power (3.3v, 5v, and GND) and working with EEPROM (ID_SD and ID_SC).
 
This time, you won’t need to think about all those other pins except GND and one GPIO pin.
 
### Programming the GPIO Pins
 
How do you tell each GPIO Pin what to do? At the most basic level, you’ll have to make commands in machine code. That’s going to be a bit too difficult for beginners.
 
Instead, for the Raspberry Pi, you can use Python or C++, which then gets compiled into machine code.
 
For this particular project, we are  using Python, as it’s easier to use.
 
## What You Need
 
- Any Raspberry Pi model that’s not the Pico (preferably the Raspberry Pi 3 Model B+ like the one in this example, but anything works), installed with the Raspberry Pi OS.An HDMI monitor and cableMouse and keyboardA phone charger (to power the Raspberry Pi)A small LEDA 250Ω resistor (can be any value close to this)A solderless breadboardx2 male-to-female jumper wires (or male-to-male if you have a header hat)

 
## How to Make Blinking LEDs
 
Let’s take this one step at a time and make one LED blink on its own.
 
- Open your terminal and type sudo apt-get install python3-rpi.gpio to install the RPi.GPIO module for Python 3.

 
- Open a text editor and type this code:

 
- Save it in a folder somewhere. The extension name should be .py. ON my Raspberry Pi, I named it “rpi-blink.py” to make it easier to find.

 
- Shut down your Raspberry Pi and remove it from all power sources.To start building the circuit, wire your LED so that there’s a resistor on either the cathode or anode, then point the cathode side to pin 7 and the anode side to pin 9 (GND).

 
Tip: to figure out the pin number, hold your Raspberry Pi in a way that the GPIO pins sit to the right. The top-left pin is pin 1, top-right is pin 2. The one below pin 1 is pin 3, then to the right of it is pin 4, and so on.
 
- Power it up again so that we can run the Python script. Open your Terminal and use cd to move to the Python file’s folder. Type:

 
to make the LED blink. 
 
Alternative: if you have Thonny Python IDE, then click on the “Run current script” button to make it run straight from the IDE.
 
- To make it stop, press Ctrl + C within the terminal. But if you’re using Thonny Python IDE, then just close the editor.

 
## How the Code Works
 
There are two things that make it work: the code and the circuit. We are starting with the code and cutting it into three parts:
 
- Import commandsSetup commandsLooped commands

 
In practice, it’s good to think of code as small functions grouped together to make bigger functions.
 
### Import Commands
 
Python normally doesn’t make it this easy to program GPIO pins. There’s a ton of stuff going on behind the scenes. The good news is that you can import the code that handles all these pesky things.
 
Take a look at lines 1 and 2:
 
These are a pair of lines that import code from something called a “Python module.”
 
import RPI.GPIO as GPIO lets you import the contents of the RPI.GPIO module and lets you use the GPIO keyword to call a function related to RPI.GPIO.
 
On the other hand, from time import sleep lets you import the sleep() function from Python’s built-in time module. This lets you delay the next line of code for a given number of seconds.
 
### Setup Commands
 
Some code has to be “set up” or defined in such a way because it’s used by other code to do complex logic. We’ll call these setup commands.
 
Unlike import commands, setup commands do not “import” code from external modules. They import them from the modules you’ve already imported.
 
As an example, GPIO.setwarnings(False) imports the .setwarnings() function from the RPI.GPIO module, which was previously defined as GPIO. This function stops a trigger warning when you run the code. It’s set to True by default.
 
To explain the other two, we are continuing with GPIO.setmode(GPIO.BOARD). That tells RPI.GPIO what kind of pinout you’re going to use. There are two types: BOARD and BCM. The BOARD pinout lets you pick pins based on their numbers. Meanwhile, the BCM pinout bases it on their Broadcomm SOC Channel designation. To keep things short, BOARD is easier to use because it’s always the same no matter which Raspberry Pi model you use. BCM, on the other hand, tends to be different from model to model.
 
Lastly, we have GPIO.setup(7, GPIO.OUT, initial=GPIO.LOW)that uses the .setup() function, which asks you three things: the pin number, its designation, and its initial value. The pin number we’re using here is pin number 7. We’re supposed to set it into an output pin and make sure that it starts out as LOW. Without this, the Raspberry Pi will never know what to do with pin 7.
 
### Looped Commands
 
This one’s the cool part. Looped commands let you tell the Raspberry Pi to do things. We started this loop with while True:, which loops the next lines of code around forever.
 
There were three functions in the loop: GPIO.output(), print(), and sleep().
 
- GPIO.output() takes an output pin and sets it to either HIGH or LOW. If you thought about changing which pin to use on your Raspberry Pi, then you should have changed 7 with a pin number of your choice.print() makes it print something out on the console. It takes in a string, number, or variable that contains the previous two.sleep() pauses the whole program for a certain number of seconds. Use a number smaller than 1 to make it pause for less than a second.

 
### The Circuit
 
Now that you know how the code works, let’s take a look at the circuit. The code makes a circuit by connecting pin 7 to GND. When pin 7 is on HIGH, it emits 3.3V that passes through the resistor and LED, then enters GND. This becomes a complete circuit and is why the LED lights up.
 
But what happens when pin 7 is on low? The 3.3V goes down to around 0V. This way, no electricity passes through the LED, so it doesn’t light up. You can think of pin 7 as a sort of a switch, as it turns the circuit either on or off.
 
## Let’s Make More LEDs Blink!
 
Now that you know what makes things work, let’s modify our code a little to make it run two LEDs.
 
For this, you’ll just need to add two more LEDs of any color and two more 250Ω resistors.
 
- Open your code editor again and paste this code:

 
- Save then shut down your Raspberry Pi.To wire up the circuit, for every LED you have, connect it to a resistor in series, then wire up the cathode side to the Raspberry Pi. There should be one for pin 7, another for pin 12, and the last one for pin 37. The anode side should be connected to GND. Each of these pins has a GND pin next to them. Those should be pins 9, 20, and 39.

 
Tip: if you run out of male-to-female jumper wire, you can stick a male-to-male to a female-to-female jumper wire to form a longer male-to-female jumper wire.
 
- Once you’re done, fire up the Raspberry Pi and repeat step 6 to launch the Python script.

 
## Frequently Asked Questions
 
### Why does my LED stay open when I stop the script?
 
When the Raspberry Pi reads the Python script, it reads the line before executing the command. You probably stopped it right after it read the line GPIO.output(7, GPIO.HIGH), so it wasn’t able to bring the pin to LOW first. You can leave it as is, as it will return to LOW the next time you reboot. Alternatively, make another Python script that turns the pin to LOW as soon as it runs.
 
### I placed my LED on the right pin, but it doesn't light up at all. Why?
 
There are two possible reasons: either your LED is broken or you put the cathode on the opposite side. Try turning the LED’s pins around first.
 
### Is it safe to place the LED the opposite way?
 
Yes. You can place it opposite, and the current will just not pass through. It’s a special trait among diodes – even light emitting diodes – they allow electricity to pass through on one side and not the other.
 
### Is it safe to reposition the LED while the Raspberry Pi is powered?
 
If it’s just turning the LED the opposite way, then it’s alright, and there’s no harm there. But if you are going to place the LED everywhere, there’s a chance that you might short the 5v pin to a GPIO pin. That’s going to break your board.
 
Terenz is a hobbyist roboticist trying to build the most awesome robot the world has ever seen. He could have done that already if he wasn't so busy burning through LEDs as a second hobby.
 
Our latest tutorials delivered straight to your inbox





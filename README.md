# ToDo-3-IoT
In this manual I'll describe how I turned a Arduino board and a led strip into a controllable light 
## Preparations
### Hardware
-Arduino board
-Led strip with wires
-Cable to transfer data
### Software 
-Arduino IDE
### Libraries
-Adafruit IO Arduino

#Step by step guide
## step 1: Conncecting the hardware.
Conncect the wire from 5V to 3V3
Middle wire (Din) to D5
GND wire to GND

## Step 2: Installing the libraries
Click the books icon in the left tab -> Paste this underneath library manager "Adafruit IO Arduino". Scroll down and click Install -> Install all.
## Step 3: Adafruit IO Setup
Enter this link in your browser of choice and click "get started for free". After making your account, enter the link again and click on the yellow key.

## Step 4: Adafruit IO Feed and Colorpicker 
On the site metioned previously, go to Dashboards > New Dashboard > Create New Block > Color picker. Enter feed name color and click on it. Then click create block. Pick a color with the color picker, don't worry, you can alway adjust this.

## Step 5: Make the code
In Arduino go to File > Examples > Adafruit IO Arduino > Adafruitio_14_neopixel. See the config tab at the top of the screen and click on it. Enter your credentials after the "define" tag corresponding to the data. For the WiFi it is advised to use a mobile hotspot. Go back to the other tab and adjust #define PIXEL_PIN 5 to #define PIXEL_PIN D5.

## Step 6: Activating the serial monitor
Upload your code (shortcut cmd + u).
Open the serial monitor by clicking the loop icon at the top right. Adjust the serial monitor to 115200 baud. If the upload was succesfull, you can restart the serial monitor and check if you see the following "Received HEX: #47aeb1". Now you can adjust the light with the color picker on Adafruit IO.





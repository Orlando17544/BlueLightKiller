# Blue Light Killer

Blue Light Killer adjusts the color temperature of your screen according to your surroundings using your webcam as a light sensor.

## Install

### Install the dependencies:

```bash
sudo apt-get install fswebcam libx11-dev libxrandr-dev
```

Install Xsct: https://github.com/faf0/sct

Install ImageMagick: https://imagemagick.org

Download the executable called blueLightKiller and execute: 

```bash
chmod +x blueLightKiller
./blueLightKiller
```

## Setup

In order to achieve better results you have to calculate the brightness in daylight (12pm preferably) and adjust the color temperature with something you feel comfortable.

To calculate the brightness download the executable called calculateBrightness and execute:

```bash
chmod +x calculateBrightness
./calculateBrightness
```

Then adjust the color temperature with something you feel comfortable(a possible starting value is 5000):

```bash
xsct 5000
```

When you know your brightness and color temperature in daylight, modify the variables called DAYLIGHT_BRIGHTNESS and DAYLIGHT_TEMPERATURE in the file blueLightKiller with your own values.

Repeat the same steps for the night(recommended value to start for color temperature is 1900), and modify the variables called NIGHTLY_BRIGHTNESS and NIGHTLY_TEMPERATURE in the file blueLightKiller with your own values.

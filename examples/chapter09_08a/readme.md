# Example Chapter09_08a
## Controlling an RGB LED of type WS2812

Example chapter09_08a utilizes object oriented programming techniques
to control an RGB LED.

This example uses essensially the tame programming techniques as in the previous example chapter09_08
to control an RGB LED, but with a sligthly modernized LED-class hierarchy.
The main difference, however, is that a _digitally_-controlled industry-standard
RGB LED of type WS2812 is used. In addition, the color transitions
at and around $255~\text{bits}$-RGB are emphasized providing longer-lasting
hues near the turning points.

## Controlling the WS2812

The WS2812 RGB LED is controlled by a very specifically timed,
novel digital signal. In this signal, each of the $24$ RGB
color bits is set to the value $1$ or $0$ depending on the
half-width of a low/high signal pair.

In this example (as in most other examples), both a hardware
version for the target system as well as a simlulated PC
version are available. For this exercise, it was
decided to implement a rather detailed PC simulation
using old-school traditional Win32-API programming.

## Application Description

Color hues of RGB blend in a smooth fashion around the entire
spectrum to produce the appearance of slowly varying colors.
The user LED is simultaneously toggled at the usual $\frac{1}{2}~\text{Hz}$.

### Enhanced RGB-Color-Light-Show

The RGB-color-light-show in example chapter09_08a (this example)
differs slightly from the one in example chapter09_08 (the previous example).

In this example the color transitions are a bit lenghtier in time
($30~\text{ms}$ as opposed to $20~\text{ms}$). Also the color transitions
at and around $255~\text{bits}$-RGB
have been lengthened for color emphasis near the turning points.

This enhanced RGB-color-light-show can be found in the file
[`app_led.cpp`](./src/app/led/app_led.cpp).

### Windows Simulation

The chapter09_08a Win32-API simulation in its Windows-based
application is shown in action in the image below.

![](./images/rgb_led_wnd_09_08a.jpg)

## Hardware Setup

In this particular example, we have simply used a commercially-available
Arduino-Nano placed on a breadboard. The wiring to the industry-standard
WS2812 RGB breakout board is simple and shown in the image below.

The hardware setup is pictured in the image below in action.
There are two pictures showing two different colors eminating
from the bright RGB LED of type WS2812.

![](./images/board09_08a_green.jpg)
![](./images/board09_08a_blue.jpg)
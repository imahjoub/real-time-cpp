# Example Chapter09_07
# Controlling a Seven Segment Display

Example chapter09_07 makes use of object oriented
programming methods to control a seven segment display.

# Controlling the RGB LED

In this example, port pins are used to control a
seven segment single-character display.

In this example (as in most other examples), both a hardware
version for the target system as well as a simlulated PC
version are available.

# Application Description

The sixteen hexadecimal digits <img src="https://render.githubusercontent.com/render/math?math=0123456789AbCdEF">
are displayed sequentially, one digit per second.
The dot (period, or decimal point) is toggled
on and off for successive groups of 16 hexadecimal digits.
The user LED is simultaneously toggled at the usual 1/2Hz.
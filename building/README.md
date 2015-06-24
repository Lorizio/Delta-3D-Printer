# Instructions

## Structure
(https://github.com/Lorizio/Delta-3D-Printer/blob/master/img/parts.jpg)

You can find the DXF files as blueprints in the DXF_files folder (credits to John Nicholson). They are very useful, specially if you can benefit the use of a laser cut machine. Use them to cut the MDF panels.

Watch Jonathan Keep's video to have an idea of how to assemble every parts together.
https://www.youtube.com/watch?v=MYd_AmkCWfM


## Electronics

### Endstops
Take the wires from the Ultra Set labeled "ENDSTOP". You can cut the red ones out. 

[img]

For each endstop, connect the blue wire to the endstop tip labeled normally closed (NC), and connect the black wire to the endstop tip labeled (COM).

Connect the 3 sets of wires as the following :

### Motors
Take the wires from the Ultra Set labeled "MOTOR" and solder each wire with each matching color wire of the step motor.

On the Arduino Board you need to configure the motor component. Jonathan Keep gives the following advice :

> Stepper motor tuning : Each stepper motor driver board has two star headed adjustment screws. [...] I have found turning the flat side [clockwise] to around three o’clock is strong enough without the motors getting too hot during continues printing. I am not quite sure what the lower screw is for but on the fabster3D EBay webpage they suggest leaving them turned fully anticlockwise. 


### Thermostat
The Ultra Set supply a very small and thin thermostat. Take the wires labeled "THERM" and solder them to the thermostat. This is necessary as the Ultra Set was thought to work with hot material and has mandatory security check systems. 

### Arduino board connections
Take from the Ultra Set the following :

- LCD screen
- SD Card
- The "L" shaped small board
- Arduino board
- The two large cables for connecting the LCD screen

When facing the Arduino board, you should see the power socket in the bottom left corner. Connect the wires from the motors, the wires from the endstops and the L shaped board as the following :

(photos credits to Jonathan Keep)

[img]

[img]

Connect the thermostat in the T0 location, just under the endstops pin.
Finally connect the two large cables between the LCD screen and the L shaped board, and put the SD card in behind the LCD screen.


### Power supply
Cut the end of the XBOX power brick and connect the wires as the following :

![ALT TEXT](https://github.com/Lorizio/Delta-3D-Printer/blob/master/img/Board_alimentation.jpg)


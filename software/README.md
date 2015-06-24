# All about software

## Driver and important steps
Connect the Arduino board to your computer. Running Windows, it should finish install itself after 2 minutes without you needing anything to do in particular (make sure you are connected to Internet so that Windows Update can download the driver). 
_If you Windows is displaying any error when connecting the board you will need to manually install the driver. Check the Arduino website for more informations._

For later use you need to know which COM port was the Arduino board installed on. You can find this information checking the properties of the board in the "Devices and Printers" from the Control Panel. Write it down. For example, mine was installed using the port COM3.


## Communication
Apart from the 3D software modeling (see below), you will need two important software that you can download right now : [Arduino](https://www.arduino.cc/en/Main/Software) and [Repetier Host](http://www.repetier.com/download/)


### Firmware
In the Arduino folder provided in this repository you can find the firmware that you need to install on the board once. 

If the dimension of your printer do not match the components given in the provided list you will need to adjust some [settings](http://solidutopia.com/marlin-firmware-user-guide-basic/). Otherwise everything is already configured and you can do the following :

1. Double click __CeramicPrinter_MarlinLCD.ino__.
2. Click on "Tools" - "Board: "Arduino Mega or ..." and choose "Arduino Mega or Mega 2560"
3. Click on "Tools" - "Port" and you should see the corresponding port I mentioned before, namely COM3 in my case.
4. Click the "Upload" button.
5. When Arduino finishes the verification process and the upload process, you can close Arduino.





## Shapes


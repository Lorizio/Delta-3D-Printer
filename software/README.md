# Software

## Driver and important steps
Connect the Arduino board to your computer. Running Windows, it should finish install itself after 2 minutes without you needing to do anything in particular (make sure you are connected to Internet so that Windows Update can download the driver). 
_If you Windows is displaying any error when connecting the board you will need to manually install the driver. Check the Arduino website for more informations._

For later use **you need to know which COM port was the Arduino board installed on**. You can find this information checking the properties of the board in the "Devices and Printers" from the Control Panel. Write it down. For example, mine was installed using the port COM3.


## Communication
Apart from the 3D software modelling (see below), you will need two important software that you can download right now : **[Arduino](https://www.arduino.cc/en/Main/Software)** and **[Repetier Host](http://www.repetier.com/download/)**


### Firmware
In the Arduino folder provided in this repository you can find the firmware that you need to install on the board once. 

If the dimension of your printer do not match the components given in the provided list you will need to adjust some [settings](http://solidutopia.com/marlin-firmware-user-guide-basic/). Otherwise everything is already configured and you can do the following :

1. Double click __CeramicPrinter_MarlinLCD.ino__.
2. Click on "Tools" - "Board: "Arduino Mega or ..." and choose "Arduino Mega or Mega 2560"
3. Click on "Tools" - "Port" and you should see the corresponding port I mentioned before, namely COM3 in my case.
4. Click the "Upload" button.
5. When Arduino finishes the verification process and the upload process, you can close Arduino.

You won't be needing Arduino anymore unless you want to adjust some settings about the printer dimensions and endstops configuration.

### Slicing and sending
The extruder of the printer needs to follow a path in space. This path is computed by a software called a __slicer__. Repetier Host is a powerful software that integrates such a tool (Slic3r).

_We need to configure Repetier Host and Slic3r_:

First of all, open Repetier Host.

#### Repetier Host
Hit CTRL+P to open the printer settings (or click on "Configuration" in the menu and select "Printer settings"). Enter a name for your printer in the top textbox and copy the settings from the following screenshots :

![ALT TEXT](https://github.com/Lorizio/Delta-3D-Printer/blob/master/img/Connection.JPG)
![ALT TEXT](https://github.com/Lorizio/Delta-3D-Printer/blob/master/img/Printer.JPG)
![ALT TEXT](https://github.com/Lorizio/Delta-3D-Printer/blob/master/img/Extruder.JPG)
![ALT TEXT](https://github.com/Lorizio/Delta-3D-Printer/blob/master/img/Printer_size.JPG)
![ALT TEXT](https://github.com/Lorizio/Delta-3D-Printer/blob/master/img/Advanced.JPG)

Click OK to apply settings.


#### Slic3r
1. From the main Repetier Host click the "Slicer" tab on the right. 
2. Select "Slic3r" from the "Slicer" drop menu and hit the "Configuration" button.
3. In the new opened window, click "File" from the menu and select "Load Config ..."
4. Select the **config.ini** provided in this repository in the Slic3r folder.

**_Note : Slic3r won't permanently save the new config unless you hit the "Save" icon in every section._**

You can close the Slic3r window.


### It's alive
Your printer should be ready to use if you followed all the steps mentioned above. Close Arduino and Repetier Host, disconnect the board from your computer.

To make sure everything works as expected always do the following when using the printer:
1. Connect the USB cable from the Arduino board
* The board should light up.
2. Connect the power cable of the board to current (you might want to use a multi-socket plug with an ON/OFF button).
3. Launch Repetier Host.
4. Use the button "Connect" in the top left corner to connect to the printer. It should turn green when successfully connected.

You are now ready to print some 3D files in the STL format (see "Shapes" section below).
To do so, do the following :

0. __Connect to the printer__. In the main Repetier Host window, check that you are connected to the printer by verifying that the "Connect" button is green. If it's not, follow the latter advice.
1. __Import the object__. In the right panel, select the first tab labelled "Object Placement". Import the desired shape to print using the "+" button. You can import any STL file and make them bigger, crop them and move them as you want. 
2. __Slice it__. In the third panel labelled "Slicer", hit the big button called "Slice with Slic3r". 
	* The fourth tab should then open and display the time it will take for the printer to print the object and some other informations.
**_Be ready to push the __Reset__ button on the Arduino board in case of any unwanted behaviour due to bad settings_**
3. __Launch it__. Hit the "Play" button and watch your printer moving.



## Shapes


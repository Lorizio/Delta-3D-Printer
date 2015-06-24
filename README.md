# Delta 3D Printer

[![IMAGE ALT TEXT](https://github.com/Lorizio/Delta-3D-Printer/blob/master/img/Video.png)](https://vimeo.com/131369209)


## Project description
Model the world in a thousands possible ways, being the architect of your environment, those are the ideas of 3D printing. The recent buzz for this type of modern printing created a real phenomenon supported by countless enthusiasts, with a constant growing community trying to improve and share their knowledge about this new innovating mean of creation.
This project is one of the many that participates to the elaborated questioning of 3D printing. It investigates the art power of such a complex machinery and confirms the renaissance of third millennium craftsmen. This project gives the hints for building a homemade Delta Printer. Using clay and a common air compressor it is possible to design complex shapes effortless. 

This printer is powered by a single Arduino board and a manually controlled air compressor to extrude the printing material. Three axis on which are sliding three mounters support the extruder at the center. There is one motor per axis, positioned at the top. This printer makes use of three endstops to calibrate itself before every printing. They are positioned at the top of each axis under the motors.

[Jonathan Keep's work](http://www.keep-art.co.uk/index.htm) was a very good support and I thank him a lot for his guidelines, especially about electronic topic.


## Repository content
There are three main topics :
* [**Building**](https://github.com/Lorizio/Delta-3D-Printer/tree/master/building).
Building a delta 3D printer from scratch, create the necessary components, connect the electronics together and the power connection configuration.
* [**Software**](https://github.com/Lorizio/Delta-3D-Printer/tree/master/software).
The drivers, the communication tools between the computer and the printer, the firmware, the required softwares, the slicing of objects and the settings of the printer.
* [**Printing Material**](https://github.com/Lorizio/Delta-3D-Printer/tree/master/printing_material).
Some requirements and guidelines about printing with clay.

 A list of the required components with a corresponding URL for easy internet finding is available for a total price of less than 300$ (see __what-you-need.odt__).
 
### Process
 
 The whole process is the following :
 
 1. Build the printer 
 2. Connect the electronics
 3. Set up the firmware
 4. Set up the printer settings
 5. Print.
 
 
 Building the printer implies dealing with soldering wires. Corresponding tools are thus needed. A laser cut machine can come in handy to facilitate the process of cutting MDF panels.
 
 The two key links of the above string are the firmware and the printer settings : 
> The firmware must be adapted to correspond to the printer dimensions such as the length of the arms and the possible angle of some particular parts. This is done using Arduino (see [Software](https://github.com/Lorizio/Delta-3D-Printer/tree/master/software)). More details [here](http://www.repetier.com/firmware/v091/) and [here](http://www.repetier.com/documentation/repetier-firmware/rf-installation/). 
 > The printer settings must match the capacity of the printer (speed and size among others). 
 
_If the printer you are dealing with is essentially the same as the one in here (i.e. was made using the provided list) you shouldn't have to configure anything._



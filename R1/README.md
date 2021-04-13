
Custom arduino:
-------------------
This is a custom development board based on the Arduino pro, uno and pro micro with some aditional features no present in those boards, and while some of them are unnecessary some can be helpfull for quick deployment of soultions and reducing wires while prototyping.
This project is completly open source and the only thing I ask for is feedback.

![](/R1/imgs/board_img.PNG)
![](/R1/imgs/PCB_img.PNG)

Repository Contents:
-------------------
* **EasyEDA** - Sopurce files (schematic and PCB).
* **FabFiles** - Fabrication files for the R1.
* **R1_Shield** - Shield template for the R1.
* **imgs** - Images of the board.

Product Features:
----------------
**R1 Features:**
 - ATmega32U4 running at 5V/16MHz.
 - Supported in the Arduino IDE.
 - On-Board reversible USB-C connector for programming and power.
 - 9x 10-bit ADC pins
 - 12x Digital I/Os (5 are PWM capable).
 - Rx and Tx Hardware Serial Connections
 - Integrated reset button.
 - 5 to 9V input voltage range.
 - Stackable female headers.
 - Fits a standard breadboard.
 - Dedicated XH-2A (grove) power input.
 - Toggable Pull-up/Pull-Down/No integrated resistors in all digital pins.
 - Builtin NEOPIXEL
 - Extra power pins, both 5 and 3v
 
R1 Know Issues as of commit:
----------------
 - Issues with neopixel (WS2812B-Mini):
    - For ease of use and acording to the docs it should be on pin D6.
	 - There's no way to disconnect the LED, a switch must be added for R2.
	 - Theres no Dout for the LED. signal out pin should be added for R2.
 - Pin issues:
	 - Arrangment of pins could be better.
	 - Pin 7 and 8 are not connected.
 - Genreal issues:
	 - Improve SilkLayer.
	 - Fix GND net.
	 - Change SilkLayer board name to "Quick Dev R2".
	 
	 Suggested pin arrangement:
![](/R1/imgs/pinarrangment.png)

License Information:
-------------------
This product is open source, no warranty is given.
Feel free to contribute and add to the project.


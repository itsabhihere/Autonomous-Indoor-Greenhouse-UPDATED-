# Autonomous Indoor Greenhouse using IoT
Monitoring the internal parameters of greenhouse like temperature and humidity and controlling the devices remotely using IoT.

![updated](https://user-images.githubusercontent.com/62765849/103232596-ddb13b80-4960-11eb-858c-74dc65aa5a39.png)



Propose contribution to the development of a prototype of an automated greenhouse monitoring and control system. This project presents the design and development of an electronic system based on a Wi-Fi embedded microcontroller that integrates remote sensing functions rooted in the cloud computing using internet of things (IoT). The system allows the acquisition of different climatic parameters in an agricultural greenhouse and in addition, this electronic system achieves the remote controlling of climatic parameters, by cloud computing solutions (internet of things). 

## Introduction:
The invention of new technologies in the domain of information science and communication has stamped its benefits for different applications. Specifically the applications of IoT in agriculture is ever expanding hugely, as it offers a well-controlled and automated farm for the farmers, better forecast of weather and crop yields for the agriculturists and knowledge on the consuming products for the common people. As in one side the designer food products count is increasing significantly, and it is also our responsibility to preserve and produce the natural food yields in well and faster scale. Here, we need the deployment of a fully-equipped and hence a well-organized greenhouse which gives various benefits for better agriculture production. Greenhouses provide constrained shelter and a controlled environment for the food crops, by providing the required temperature and aeration. This temperature controlled atmosphere gives the plants a healthy environment for its good yield in greenery, flowers and fruits. Stunted growth in plants seen in open-air nurture, delays the plant produce period. This can be extremely avoided with the use of a greenhouse as it helps the plants to maintain moisture in its surrounding and in the soil as well. For the growing and end of a plant’s normal life cycle, it requires some vital factors like light, nutrients absorbed from soil, air and water, proper temperature and humidity.
In the conventional process, the farmer has to visit the entire field regularly at odd hours to confirm the well-being of his farm, which mostly includes the switching ON/OFF motor to ensure that his plants are watered. Sometimes, the plants are not watered enough and hence essential nutrients aren’t absorbed from the soil. Sometimes, the motor pumps are left running for longer than what is necessary because of the effort involved to turn OFF the motor and hence leads to water logging, rotting of roots and deprivation of oxygen from the soil. Hence it is clearly evident that conventional process lead to improper use and wastage of the resources available. Soil erosion and salinization, eutrophication, water depletion are some problems encountered with traditional agriculture. An automated greenhouse helps to monitor the soil moisture and its nutrients levels, air moisture and macro nutrients, and light intensity through several sensors. Autonomous greenhouse enhances the management efficiency and optimizes the agricultural resources. IoT takes agriculture a step above just the traditional agricultural processes by collecting and analysis of sensed data and decision making. This process can also actuate various activities in an automated greenhouse system, which supports the farmers in various ways and conserving their efforts and time for further increasing the productivity.
The project proposes designing of greenhouse system which has various sensors for detection scheme of different parameters required for healthy growth of plants. The communication between the module and internet is done using the MQTT protocol. MQTT (MQ Telemetry Transport or Message Queuing Telemetry Transport) is an open OASIS and ISO standard (ISO/IEC 20922) lightweight, publish-subscribe network protocol that transports messages between devices. Using soil moisture sensor, HDT11 sensor, LDR sensor for detecting the sensor readings which are the computed using the arduino ide and based of these input data from the sensors the automation of the greenhouse is done. The relays are connected with water pump, fan and lights which are controlled with the help of microcontrollers used such as the arduino uno and NodeMCU which helps our project to automate and also connect to the online services, so that we can control our greenhouse from anywhere in the world with the help of simple graphical interface made on adafuit io, and the greenhouse can also be controlled from any MQTT service supporting mobile application.

## OBJECTIVE 
The main objective of this Project is to make a simple, autonomous greenhouse system for controlling the different parameters of the greenhouse using Arduino Uno, Nodemcu and Internet of things. It also provides the facility to monitor and control the greenhouse from anywhere in the world. The system mainly concentrates on how to control lighting, water level, temperature fluctuations and many, which can help humans to grow plants and vegetables easily in their Home. It also improves Convenience, comfort, energy efficiency and time because of being autonomous.  To Build miniature greenhouse which is equipped with automatic monitoring and controlling system  Send/Monitor the status of the Greenhouse system by sending the data through IOT Website.  Change the status (turn ON/OFF) of the device upon receiving commands through Website or Android application.  To maintain the history of parameter records.  Ease of accessing and simplicity on maintenance.  Advanced connectivity of physical objects over a wide network.  Display status of the Greenhouse in an OLED screen placed on the structure of the greenhouse.  It focuses on saving water, increasing efficiency and reducing the environmental impacts on plants production.

## Advantages
 <ul>
 <li> Total automation of greenhouses / nurseries / bio tech parks. 
 <li> Remote device control, can be controlled from anywhere in the world. 
 <li> Can be used domestically. 
 <li> Easy to use, install, operate & troubleshoot. 
 <li> Useful for greenhouse owners, small scale farmers. Low cost setup. 
 <li> No Manual intervention needed.
 </ul>

 ## Components: 
 ### Arduino UNO: 
 The Arduino uno is open source microcontroller board based on the Microchip ATmega-328P microcontroller and developed by Arduino.cc. The board is equipped with sets of digital and analog input/output (I/O) pins that may be interfaced to various expansion boards (shields) and other circuits. The board has 14 digital I/O pins (six capable of PWM output), 6 analog I/O pins, and is programmable with the Arduino IDE (Integrated Development Environment), via a type B USB cable. It can be powered by the USB cable or by an external 9-volt battery, though it accepts voltages between 7 and 20 volts.

 ![arduino correct](https://user-images.githubusercontent.com/62765849/103232942-ce7ebd80-4961-11eb-9899-4a86ee3bc942.png)

#### General pin functions
 <ul><li> LED: There is a built-in LED driven by digital pin 13. When the pin is high value, the LED is on, when the pin is low, it is off. 
 <li> VIN: The input voltage to the Arduino/Genuino board when it is using an external power source (as opposed to 5 volts from the USB connection or other regulated power source). You can supply voltage through this pin, or, if supplying voltage via the power jack, access it through this pin. 
 <li> 5V: This pin outputs a regulated 5V from the regulator on the board. The board can be supplied with power either from the DC power jack (7 - 20V), the USB connector (5V), or the VIN pin of the board (7-20V). Supplying voltage via the 5V or 3.3V pins bypasses the regulator, and can damage the board. 
 <li> 3V3: A 3.3 volt supply generated by the on-board regulator. Maximum current draw is 50 mA. 
 <li> GND: Ground pins. 
 <li> IOREF: This pin on the Arduino/Genuino board provides the voltage reference with which the microcontroller operates. A properly configured shield can read the IOREF pin voltage and select the appropriate power source, or enable voltage translators on the outputs to work with the 5V or 3.3V. 
 <li> Reset: Typically used to add a reset button to shields that block the one on the board.
</ul>

#### Special pin functions
 Each of the 14 digital pins and 6 analog pins on the Uno can be used as an input or output, under software control (using pinMode(), digitalWrite(), and digitalRead() functions). They operate at 5 volts. Each pin can provide or receive 20 mA as the recommended operating condition and has an internal pull-up resistor (disconnected by default) of 20-50K ohm. A maximum of 40mA must not be exceeded on any I/O pin to avoid permanent damage to the microcontroller. The Uno has 6 analog inputs, labeled A0 through A5; each provides 10 bits of resolution (i.e. 1024 different values). By default, they measure from ground to 5 volts, though it is possible to change the upper end of the range using the AREF pin and the analogReference() function. In addition, some pins have specialized functions: 
<ul> 
<li> Serial / UART: pins 0 (RX) and 1 (TX). Used to receive (RX) and transmit (TX) TTL serial data. These pins are connected to the corresponding pins of the ATmega8U2 USB-to-TTL serial chip. 
 <li> External interrupts: pins 2 and 3. These pins can be configured to trigger an interrupt on a low value, a rising or falling edge, or a change in value. 
 <li> PWM (pulse-width modulation): pins 3, 5, 6, 9, 10, and 11. Can provide 8-bit PWM output with the analogWrite() function. 
 <li> SPI (Serial Peripheral Interface): pins 10 (SS), 11 (MOSI), 12 (MISO), and 13 (SCK). These pins support SPI communication using the SPI library. 
 <li> TWI (two-wire interface) / I²C: pin SDA (A4) and pin SCL (A5). Support TWI communication using the Wire library. 
 <li> AREF (analog reference): Reference voltage for the analog inputs. 
 </ul>

 #### Technical Specifications 
 <ul>
 <li> Microcontroller: Microchip ATmega328P 
 <li> Operating Voltage: 5 Volts 
 <li> Input Voltage: 7 to 20 Volts 
 <li> Digital I/O Pins: 14 (of which 6 can provide PWM output) 
 <li> UART: 1 
 <li> I2C: 1 
 <li> SPPI: 1 
 <li> Analog Input Pins: 6 
 <li> DC Current per I/O Pin: 20 mA 
 <li> DC Current for 3.3V Pin: 50 mA 
 <li> Flash Memory: 32 KB of which 0.5 KB used by bootloader 
 <li> SRAM: 2 KB 
 <li> EEPROM: 1 KB 
 <li> Clock Speed: 16 MHz  Length: 68.6 mm 
 <li> Width: 53.4 mm 
 <li> Weight: 25 g
 </ul>
 
 ### NodeMCU (ESP8266 WIFI MODULE):
  The NodeMCU (Node MicroController Unit) in figure 1 is an open source software and hardware development environment that is built around a very inexpensive System-on-a-Chip (SoC) called the ESP8266. The ESP8266, designed and manufactured by Espressif Systems, contains all crucial elements of the modern computer: CPU, RAM, networking (wifi), and even a modern operating system and SDK. NodeMCU in this prototype used a microcontroller module with a Wi-Fi system which was programmed using Arduino IDE. The version of NodeMCU we are using V.3 board or commonly also called ESP-12E.







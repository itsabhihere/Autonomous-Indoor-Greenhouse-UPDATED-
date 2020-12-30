# Autonomous Indoor Greenhouse using IoT
Monitoring the internal parameters of greenhouse like temperature and humidity and controlling the devices remotely using IoT.

![updated](https://user-images.githubusercontent.com/62765849/103232596-ddb13b80-4960-11eb-858c-74dc65aa5a39.png)



Propose contribution to the development of a prototype of an automated greenhouse monitoring and control system. This project presents the design and development of an electronic system based on a Wi-Fi embedded microcontroller that integrates remote sensing functions rooted in the cloud computing using internet of things (IoT). The system allows the acquisition of different climatic parameters in an agricultural greenhouse and in addition, this electronic system achieves the remote controlling of climatic parameters, by cloud computing solutions (internet of things). 

## Introduction:
<ul>
  <li>In today’s greenhouses, many parameter measurements are required to monitor and control for the good quality and productivity of plants. But to get the desired results there are some very important factors which come into play like Temperature, Humidity, Light and Water, which are necessary for a better plant growth. Keeping these parameters in mind, we are building an automatic greenhouse controlling and monitoring system over Arduino UNO, ESP8266 Module or NodeMcu and different sensors. 
  <li>This system is very efficient for growing good quality plants. The other important part of this project is that it is fully automatic. Arduino sends the information about different parameters such as temperature, humidity, light intensity, soil moisture. The module automatically turn on/off the appliances (fans, artificial lights and water pump) that are connected with circuit for controlling the greenhouse parameters. 
  <li>In this project we use GUI (Graphical User Interface) of adafruit IO services to make a interactive interface having on/off buttons, different gauges and graphs to control and monitor the Autonomous greenhouse system using internet and iot, which can be accessed from any web browser. 
  <li>The system mainly concentrates on how to control lighting, water level, temperature fluctuations and many, which can help humans to grow plants and vegetables easily in their home. It also improves Convenience, comfort, energy efficiency and time because of being autonomous.
</ul>  

![Untitled](https://user-images.githubusercontent.com/62765849/103345077-6ab9d900-4ab6-11eb-85d2-10880250d493.png)
In this circuit we have used DHT11 sensor for detecting the temperature and humidity of the surroundings of plants, LDR sensor to measure the light intensity through which the status of the lights will change to ON/OFF according to the programming of the micro-controllers, soil moisture sensor to measure the soil moisture level, all the sensors are connected to the Arduino uno, whereas, a 4-channel relay is connected to Nodemcu V3 which is controlled both with the arduino programming and the web interface on adafruit IO, a OLED screen to display the live sensor reading. The sensors will collect the data from its surroundings and soil, then further send the data from arduino uno to nodemcu with the help of serial communication. The nodemcu will further connect the project with internet and its cloud servers and we can easily monitor/control the greenhouse system.


## OBJECTIVE 
The main objective of this Project is to make a simple, autonomous greenhouse system for controlling the different parameters of the greenhouse using Arduino Uno, Nodemcu and IOT (Internet of things). It also provides the facility to monitor and control the greenhouse from anywhere in the world. The system mainly concentrates on how to control lighting, water level, temperature fluctuations and many, which can help humans to grow plants and vegetables easily in their Home. It also improves Convenience, comfort, energy efficiency and time because of being autonomous. 
<ul>
<li> To Build miniature greenhouse which is equipped with automatic monitoring and controlling system 
<li> Send/Monitor the status of the Greenhouse system by sending the data through IOT Website. 
<li> Change the status (turn ON/OFF) of the device upon receiving commands through Website or Android application. 
<li> To maintain the history of parameter records. 
<li> Ease of accessing and simplicity on maintenance. 
<li> Advanced connectivity of physical objects over a wide network. 
<li> Display status of the Greenhouse in an OLED screen placed on the structure of the greenhouse. 
<li> It focuses on saving water, increasing efficiency and reducing the environmental impacts on plants production.
</ul>

## Advantages
 <ul>
 <li> Total automation of greenhouses / nurseries / bio tech parks. 
 <li> Remote device control, can be controlled from anywhere in the world. 
 <li> Can be used domestically. 
 <li> Easy to use, install, operate & troubleshoot. 
 <li> Useful for greenhouse owners, small scale farmers. Low cost setup. 
 <li> No Manual intervention needed.
 </ul>

## Working
 <ul>
<li>The main brain of this project is the Arduino, It is a closed loop system in which the different parameters of the greenhouse are controlled with the microcontroller. 
<li>The microcontroller is fed with program code which process the input data from sensors and automates the greenhouse.
<li>In-order to automate the growing process of plants we use the data from different sensors which are then processed with the help of program code and then the parameters of the greenhouse are maintained.
<li>The data being exchanged between the two microcontrollers i.e. arduino uno and nodemcu is sent/received in the form of an array with the help of SoftwareSerial library in arduino IDE.
<li>Now, as the automation process is handled by the Arduino UNO board, the communication with the internet is done through another module which is known as Nodemcu, which helps the Arduino to connect with internet and process the data in such a from that is easy to control and manage.
<li>The arduino uno and nodemcu will communicate to each other with the help of Serial Communication and libraries such as SoftwareSerial library and ArduinoJson Library.
<li>After, receiving the data from uno board, the nodemcu controls the relays. Water pump, fan, lights which are connected with the relays are controlled using both the microcontroller and adafuit io or mqtt based mobile application.  
</ul>

## Adafruit IO
<ul>
<li>MQTT, or message queue telemetry transport, is a protocol for device communication that Adafruit IO supports .
<li>Adafruit IO is a system that makes data useful. Its focus is on establishing a connection between a hardware and software, and allowing simple data connections with little programming required.
<li>IO includes client libraries that wrap our MQTT APIs.
<li>IO is built on Ruby on Rails, and Node.js.
<li>Adafruit.io is a cloud service.
</ul>

![1](https://user-images.githubusercontent.com/62765849/103342541-c16fe480-4aaf-11eb-86da-4ca4f61be3e8.png)

<hr>

![adafruit](https://user-images.githubusercontent.com/62765849/103342674-2592a880-4ab0-11eb-8385-0860f53072b3.PNG)

## Components: 
<ul>
<li>Arduino UNO
<li>NodeMCU
<li>Oled display
<li>DHT11 temperature & humidity sensor
<li>Soil moisture sensor
<li>LDR sensor
<li>Water Pump
<li>4-channel relay
<li>Lights 
<li>Fan
</ul>

### Arduino UNO: 
 The Arduino uno is open source microcontroller board based on the Microchip ATmega-328Pmicrocontroller and developed by Arduino.cc. The board is equipped with sets of digitaland analog input/output (I/O) pins that may be interfaced to various expansion boards(shields) and other circuits. The board has 14 digital I/O pins (six capable of PWM output, 6 analog I/O pins, and is programmable with the Arduino IDE (Integrated DevelopmentEnvironment), via a type B USB cable. It can be powered by the USB cable or by an external9-volt battery, though it accepts voltages between 7 and 20 volts.
 ![arduino correct](https://user-images.githubusercontent.com/62765849/103232942-ce7ebd80-4961-11eb-9899-4a86ee3bc942.png)
 #### Pins 
 ![pins](https://user-images.githubusercontent.com/62765849/103341753-c16ee500-4aad-11eb-9881-47f3bffc1f63.PNG)

 #### Technical Specifications 
 <ul>
 <li> Microcontroller: Microchip ATmega328P 
 <li> Operating Voltage: 5 Volts 
 <li> Input Voltage: 7 to 20 Volts 
 <li> Digital I/O Pins: 14 (of which 6 can provide PWM output) 
 <li> UART: 1 
 <li> I2C: 1 
 <li> SPPI: 1 
 <li> Analog Input Pins: 6 
 <li> DC Current per I/O Pin: 20 mA 
 <li> DC Current for 3.3V Pin: 50 mA 
 <li> Flash Memory: 32 KB of which 0.5 KB used by bootloader 
 <li> SRAM: 2 KB 
 <li> EEPROM: 1 KB 
 <li> Clock Speed: 16 MHz  Length: 68.6 mm 
 <li> Width: 53.4 mm 
 <li> Weight: 25 g
 </ul>
 

### NodeMCU (ESP8266 WIFI MODULE):
  The NodeMCU (Node MicroController Unit) in figure 1 is an open source software and hardware development environment that is built around a very inexpensive System-on-a-Chip (SoC) called the ESP8266. The ESP8266, designed and manufactured by Espressif Systems, contains all crucial elements of the modern computer: CPU, RAM, networking (wifi), and even a modern operating system and SDK. NodeMCU in this prototype used a microcontroller module with a Wi-Fi system which was programmed using Arduino IDE. The version of NodeMCU we are using V.3 board or commonly also called ESP-12E.

  ![nodemcu](https://user-images.githubusercontent.com/62765849/103341251-6ee0f900-4aac-11eb-9328-5b6d237ebf15.PNG)

  #### Pins
![pins](https://user-images.githubusercontent.com/62765849/103341831-ec593900-4aad-11eb-99d1-4ff944166c50.PNG)

#### Technical Specifications
Microcontroller ESP-8266 32-bit
<ul>
  <li>NodeMCU Model: Clone LoLin 
  <li>NodeMCU Size: 58mm x 32mm 
  <li>Pin Spacing: 1.1" (27.94mm) 
  <li>Clock Speed: 80 MHz 
  <li>USB to Serial: CH340G 
  <li>USB Connector: Micro USB 
  <li>Operating Voltage: 3.3 V 
  <li>Input Voltage: 4.5V-10V 
  <li>Flash Memory/SRAM: 4 MB / 64 KB 
  <li>Digital I/O Pins: 11 
  <li>Analog In Pins: 1 
  <li>ADC Range: 0-3.3V 
  <li>UART/SPI/I2C: 1/1/1 
  <li>Wifi Built-In 802.11 b/g/n 
  <li>Temperature Range: -40C – 125C
</ul>

### OLED Display:
<ul>
<li>In order to verify the collected data locally, a small OLED Display is installed. The model used on Autonomous Indoor Greenhouse is the OLED 128 x 64 SSD 1306 I2C.

<li>The main characteristics of this display are:
 <ol>
    <li>128 pixels at horizontal and 64 pixels at vertical.
    <li>Display (8 lines of 16 characters each).
  </ol>
<li>It is a I2C display which will connect using pins:
  <ol>
    <li>SCL ==> D1 (5)
    <li>SDA ==> D2 (4)
  <ol>
</ul>

![oled](https://user-images.githubusercontent.com/62765849/103343068-22e48300-4ab1-11eb-952f-a74a1409961a.png)

### DHT11 temperature & humidity sensor:
<ul>
<li>One of most used sensors for capturing weather data is the DHT11, a digital relative humidity and temperature sensor. It uses a capacitive humidity sensor and a thermistor to measure the surrounding air, and spits out a digital signal on the data pin (no analog input pins needed).
<li>The sensor should be powered between 3.3V and 5V and will work from -40oC to +80oC with an accuracy of +/- 0.5oC for temperature and +/-2% for relative Humidity. It is also important to have in mind that the its sensing period is in average 2 seconds (minimum time between readings).
<li>The DHT11 has 3 pins:
       1. VCC (we will connect to 3.3V from UNO)
       2. Data out
       3. Ground
</ul>

![dht](https://user-images.githubusercontent.com/62765849/103343156-6ccd6900-4ab1-11eb-8dc1-525f5a791fc0.png)

### Soil moisture sensor:
<ul>
<li>The Soil Moisture sensor is used to measure the water content(moisture) of soil. The Soil Moisture Sensor uses capacitance to measure dielectric permittivity of the surrounding medium  which is the soil here. The soil moisture sensor module consists of a moisture sensor probe and LM393 Comparator.
<li>The LM393 module has 2 outputs, one digital (D0) that can be set-up using the potentiometer that exist on it and an analog one (A0). This module can be sourced with 3.3V
  The 4 pins are:
  <ol>
    <li>LM393 A0 output to A0 input of UNO
    <li>LM393 VCC to NodeMCU VCC.
    <li>LM393 GND to NodeMCU GND
    <li>LM393 D0 open.
  </ol>
<ul>

![soil](https://user-images.githubusercontent.com/62765849/103345190-b79daf80-4ab6-11eb-9359-62363eb5c3c6.png)


### LDR sensor:
<ul>
  <li>An LDR is a component that has a (variable) resistance that changes with the light intensity that falls upon it. This allows them to be used in light sensing circuits.
  <li>A LDR sensor module has 3 pins:
    <ol>
      <li> VCC (we will connect to 3.3V from UNO)
      <li> Data out
      <li> Ground
    </ol>
</ul>

![ldr](https://user-images.githubusercontent.com/62765849/103343491-304e3d00-4ab2-11eb-8ad9-69bc1fad660d.png)

### Water Pump:
This is Micro Submersible Water Pump DC 3V-5V, can be easily integrated to our project and connected with relay. The water pump works using water suction method which drain the water through its inlet and releases it through the outlet. 
![punp](https://user-images.githubusercontent.com/62765849/103343587-70adbb00-4ab2-11eb-8a37-e3b1cbcd87c0.png)

### 4-channel relay:
<ul>
  <li>The 4 Channel Relay Module is a convenient board which can be used to control high voltage, high current load such as motor, solenoid valves, lamps and AC load. It is designed to interface with microcontroller such as Arduino, PIC and etc. The relays terminal (COM, NO and NC) is being brought out with screw terminal.

  <li>The 4 channel relay has 6 pins:
    <ol>
      <li>VCC (connect to 3.3V from UNO)
      <li>4 input lines (IN1, IN2, IN3, IN4)
      <li>Ground
    </ol>
</ul>

![relay](https://user-images.githubusercontent.com/62765849/103343719-b9fe0a80-4ab2-11eb-9f4d-e22e6d46372f.png)


## PROJECT VIDEO

THANKS FOR WATCHING!!!

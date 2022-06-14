## Overview

This project covers how to setup the software and hardware to use a Bluetooth heart rate sensor to automate the speed of
a treadmill. The goal is to make it easier to train Maffetone Method, Zone Training or simular. 

Using a Bluetooth heart rate monitor, connected to an ESP32 to get the hear rate number. This number will be sent via MQTT
subscriber on the computer to log the data. At this point the user can analyze the data however they want. The heart rate number
collected on the ESP32 will be used to automate the speed of the treadmill. The user will be able to set the heart rate for their
training. The user will also be able to set the top speed they want to train at and how fast they want the treadmill to slow down
as thier heart rate reaches the target amount. 

This project will be completed as simplisically as possible for a user with some programming expierence and soldering to be
able to complete. I'll be using the Mosquitto MQTT broker, programming the ESP32 with Arduino code and programming a data logger
with python on a laptop. 

## Software Needed

- Install Mosquitto Broker

https://mosquitto.org/download/

I personally installed this in my developement windows 11 laptop, but it can be installed on win, mac and linux. SBC can 
also be used such as raspberry pi. I'll be sharing how I used the broker in an unscecure manner, but more more professional 
projects TLS can be used with this broker. 

- Install Arduino  

Install Arduino IDE 
https://www.arduino.cc/en/software

Add ESP32 to Arduino IDE 
https://docs.espressif.com/projects/arduino-esp32/en/latest/installing.html

- install graphana

grafana.com 

I use this for fancy graphs to track the data. Once installed, open web browser and open localhost:3000 and login with admin admin


## Hardware Need

- ESP32 devkit C

- ESP32 cower cable

- Polar H10 Heart Rate Monitor Chest Strap - ANT + Bluetooth, Waterproof HR Sensor for Men and Women 
https://www.amazon.com/Polar-Heart-Rate-Monitor-Women/dp/B07PM54P4N/

- Random soldering supplies and wires


# Wireless-Geo-Temperature-Mapping-System

# Introduction
This project aims to design and build a custom mobile device capable of reading various sensors, parsing data, and broadcasting the required information over Wi-Fi. The data received by a PC will be utilized to draw a temperature map based on dynamic locations (global latitude and longitude) and corresponding ambient temperatures. First, we soldered the Arduino Uno, GPS module, Wi-Fi module, Thermistor, and regulator to the PCB card appropriately. Although Arduino had 3.3 V, we reduced it to 3.3 V using a regulator, otherwise, the project would have failed due to lack of current. Arduino Uno gathers data from the NEO-6M GPS Module and NTC Thermistor and communicates serially with NEO-6M and ESP8266-01. The Wi-Fi module broadcasts data to the PC via Wi-Fi using TCP. We develop a PC program using Python3 to receive and parse data. The program creates an interface displaying dynamic locations with corresponding temperatures, forming a temperature map.


# Software
  ![image](https://github.com/user-attachments/assets/ebbd559d-ed66-4da5-93ac-1d7dcc524dea)

  ![image](https://github.com/user-attachments/assets/1d7d0cf2-0131-4e5c-b053-3a7a81492f84)


# Conclusion
We are experienced in sensor integration, serial communication, Wi-Fi networking, and, contributing to their skills in both hardware and software aspects of embedded systems. The NEO-6M GPS Module uses the NMEA standard protocol for sending data. We parsed this data with Arduino Uno. ESP8266-01 acts as a bridge, broadcasting data from Arduino to PC and vice versa. After pulling the necessary data from the NMEA codes, we packaged the code in a single line to include temperature and location information. PC and Wi-Fi module were connected to the same Wi-Fi. After getting the  IP address, we ran the code and pulled the data.

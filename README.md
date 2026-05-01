# Wearable Sensor

_**About This Project:**_

**Wearable Sensor** is a QL Plus Project developed by Briana Sepulveda, Nanda Johnson, Jessica Malakhova, and Arturo Martinez.

This project's ultimate goal is to create a device under $30 to display and measure user’s heartrate, temperature, SpO2 with 95% accuracy.

Here's a demonstration of Wearable Sensor! https://youtu.be/xxxx

_**Materials Used:**_

ELEGOO UNO R3 Board: [https://a.co/d/0aggOWlQ]

0.96" OLED i2c Display Module Screen: [https://a.co/d/0e8LvMpk]

Heart Rate Sensor Module MAX30102 (Arduino Compatible): [https://a.co/d/0g5pY85o]

120pcs Breadboard Jumper Wires 20cm Wire: [https://a.co/d/08JQEu3K]

ELEGOO Breadboard 830 Point Solderless: [https://a.co/d/044U4O8P]

18650 Battery Holder with DC Jack: [https://a.co/d/00qv2IIv]

18650 Batteries: [https://a.co/d/05ejoc3g]


_**Setup:**_

1. Go to https://www.arduino.cc/en/software/
2. Download the latest verison of the Arduino IDE [We used verison 2.3.8 at the time of building]
3. Open the "arduino-ide_X.X.X_OSNAME_64bit.exe" file
4. Press "I Agree"
5. Press "Next"
6. Press "Install"
7. After Arduino IDE downloads, Press "Finish"
8. Once Arduino IDE opens, press on the "Library Manager" icon [Highlighted in white!] <img width="89" height="602" alt="image" src="https://github.com/user-attachments/assets/b1f1d16d-c4aa-49b5-88a9-ebf055225eec" />
9. Search "Adafruit SSD1306" and Press "Install"
10. Search "SparkFun MAX3010x Pulse and Proximity" and Press "Install"
11. Open and Close the Arduino IDE to ensure the libraries are properly downloaded
12. Go back to this Github and open the "wearablesensorcode" file
<img width="762" height="289" alt="image" src="https://github.com/user-attachments/assets/2fec96d9-0d91-4a73-913b-f1754ead8525" />

13. Click in the code and press "Ctrl + A", then "Ctrl + C"
14. Go back to the Arduino IDE, click inside your workspace, press "Ctrl + A", then "Backspace", then press "Ctrl + V" to paste the code

Now, we can begin putting our Arduino, Sensor, and Screen together!

15. Cut 1 male to female wire to 2 inches in length, strip ends of the wire and connector, and solder them together to successfully shorten wires to fit in the 3D printed box.
16. Place electrical tape over any soldered connections (applicable in future steps as well)
17. Establish a common Ground by connecting the GND rail on the breadboard to a GND pin on the Arduino using a black wire
18. Cut one male to male wire and one female to female wire so that each segment is about 2 inches in length.
19. Strip the jacket at the ends
20. Twist the three leads (one male and two female) together, and solder the connection to create a signal splitter. Refer to images below <img width="959" height="719" alt="image" src="https://github.com/user-attachments/assets/684fc157-1ac5-4069-a65a-d23317c6da3a" /> <img width="871" height="831" alt="image" src="https://github.com/user-attachments/assets/d57dcba7-003e-4ecb-91e4-ef5176c413df" />


21. Connect the male end of the wire to the 3.3 V pin on the Arduino.
22. Connect the two female ends to the VCC pin on the screen and VIN pin on sensor respectively to distribute power to both the components. (Power line)
23. Connect the male end of the wire to the SDA pin on the Arduino.
24. Connect the two female ends to the SDA pins on the screen to enable I2C data communication between the Arduino and the components. (Data line)
25. Connect the male end of the second data splitter to the SCL pin on the Arduino.
26. Connect the two female ends to the SCL pins on both the sensor and the screen to synchronize data transmission. (Clock line)
27. Connect the DC Jack to the Arduino to allow the sensor and screen to be battery operated (18650 batteries).
28. If creating connection betwen DC jack and battery holder, connect dashed wire at the jack to the positive wire from the batteries. Solder the other wire at the jack to the negative wire from the batteries. Refer to image below.<img width="750" height="563" alt="image" src="https://github.com/user-attachments/assets/4a3ebee3-4488-4fd2-a674-ede2ff99d36a" />
 
Now we can begin the final assembly!

26. Download the following CAD file using the link below and 3D print the design (we used the Bamboo P1S printer and PLA). https://cad.onshape.com/documents/86e2b73f0955df2799a4342b/w/6d0c789f0a9a81bec4d81045/e/72fe08d523685dd6bc83bfe8?renderMode=0&uiState=69f517a805b22f6e38fd06c4
27. Place the Screen and Sensor in the appropriate compartments making sure to reconnect wires wires as described above.


**CONGRATULATIONS!!! 🥳 You've succesfully built your own Wearable Sensor that you can use and enjoy wherever you desire!**

Thank you so much for taking the time to build your own! Feel free to modify the project fit your needs and share your creation with others!

-- Briana Sepulveda (briana.sepulveda@my.utsa.edu), Nanda Johnson (jananda.johnson@my.utsa.edu), Jessica Malakova (jessica.malakova@my.utsa.edu), Arturo Martinez (arturo.j.martinez.ii@gmail.com)

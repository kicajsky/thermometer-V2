#Digital Thermometer V2 with clock

Power supply 2V -> Boost converter MCP1640 to 3.3V
MCU: ST F401RCT7
Sensors: 2x BS18B20, one mounted on the PCB (inside box), second external 
RTC DS3231 with EEPROM 24C32 
-----------------------------------------------------------------------------------------------------------
How it works:
There are 2 buttons. 
1 - On/Off device:
- short press to turn on.
- 0.5s press to turn off.

Auto off after 3h.

2 - switch between functions, short press to change:
DS18B20 Sensor 1 -> DS18B20 Sensor 2 -> DS3231 Clock -> Battery voltage -> Sensor 1...
---------------------------------------------------------------------------------------
Sensor priority select:
Connected sensors are automatically assigned addresses and priorities. 
- Short Jumper J2 on PCB to change priority.
---------------------------------------------------------------------------------------
Time setting:
While function clock is on display, press and hold for 2 seconds button 2.
To set hours (0-23), short press button 2. To set minutes, short press button 2
To accept time and exit, press and hold for 2 seconds button 2.
---------------------------------------------------------------------------------------
Change brightness:
While function temperature or battery voltage measure is on display, press and hold for 2 seconds button 2.
Short press button 2 to increment brightness.
Press and hold for 2 seconds button 2 to save setting.

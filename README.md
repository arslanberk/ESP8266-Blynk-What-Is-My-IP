# ESP8266-What-Is-My-IP
Use Blynk.io mobile application to get public IP address from ESP8266.

## Upload Code

1 Open [Arduino IDE](https://www.arduino.cc/en/Main/Software) and go to File > Preferences (CTRL + COMMA);
	- Add ```Additional Boards Manager URLs```: http://arduino.esp8266.com/stable/package_esp8266com_index.json
2 [Install Blynk Library](http://help.blynk.cc/getting-started-library-auth-token-code-examples/how-to-install-blynk-library-for-arduino);
3 Go to Tools > Board > Boards Manager
	- Install ```esp8266``` by ESP8266 Community
4 Go to Tools > Board
	- Select ```Generic ESP8266 Module```

IMPORTANT: Do not forget to select proper Serial Port!

## Blynk App

1 ```Value Display``` for IP address 
	- Input Pin: V1
	- Reading Rate: PUSH
2 ```Value Display``` for API in use
	- Input Pin: V10
	- Reading Rate: PUSH
3 ```Button``` for help
	- Output Pin: V2 (0-1)
	- Mode: PUSH
4 ```Button``` for clear
	- Output Pin: V3 (0-1)
	- Mode: PUSH
5 ```Button``` for wifi
	- Output Pin: V4 (0-1)
	- Mode: PUSH
6 ```Button``` for updating IP
	- Output Pin: V5 (0-1)
	- Mode: PUSH
7 ```Terminal```
	- Input Pin: V0 (0-1)
	- Add Newline: NO
	- Input Line: ON
	- Autoscroll: ON
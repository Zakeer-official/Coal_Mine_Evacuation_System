# Coal Mine Evacuation System Using Multi-Sensor Control

# Abstract:
Embarking on an unprecedented journey into coal mine safety, our project unveils an ingenious evacuation system powered by Raspberry Pi and Grove Pi. Picture a network of cutting-edge sensors and smart devices working harmoniously to safeguard miners from potential dangers. From monitoring temperature fluctuations and air quality to alerting in case of sound anomalies, this system creates a fortified shield of protection. When emergencies strike, piercing alarms kick into action, guiding miners to safety. Imagine a dynamic LCD display providing real-time information, pinpointing the locations of life-saving emergency kits. Not stopping there, our system even adapts to ambient lighting. Witness a game-changer in safety technology that sets the new standard for hazardous environments, all wrapped up in a customizable package tailored to specific needs.

# Introduction:
Venturing into the depths of coal mines, our project emerges as a technological sentinel for safety. Welcome to the realm of the "Coal Mine Evacuation System" - an innovation that fuses Raspberry Pi and Grove Pi prowess to reimagine safety within mining. Through an intricate web of sensors and intelligent alerts, we navigate miners through challenges, ushering in an era of real-time protection and responsive guidance. Join us on a journey that marries cutting-edge technology with unwavering dedication to miners' safety.

# Hardware Required:
1.	Raspberry Pi 3
2.	Grove Pi Sensors
Sensors and Actuators: 
•	LEDs (Red, Blue, Green) 
•	Sound Sensor 
•	Temperature and Humidity Sensor 
•	Light Sensor 
•	Button 
•	Ultrasonic Sensor 
•	Rotary Angle Sensor 
•	Buzzer 
•	RGB LCD Display 
•	Air Quality Sensor 
•	Relay
•	Power Supply
•	Jumper Wires(In case of ethernet)


![image](https://github.com/Zakeer-official/Coal_Mine_Evacuation_System/assets/102544273/975cae1b-b2de-401d-adf1-e1a90f4d371f)


 
# Initialization:
<pre>
Initialize sensors (LEDs, Sound, Temperature/Humidity, Light, Button, Ultrasonic, Rotary, Buzzer, LCD Display, Air Quality).
Initialize communication (Email, LCD, etc.).
Set constants (Thresholds, Emergency Kits Location, etc.).
Display system startup message on the LCD.
System Activation:
Wait for the button press.
Display "System Activated" on the LCD.
Enter the main loop.
Main Loop:
Read sensor data (Temperature, Humidity, Sound, Light, Distance, Angle, Air Quality).
Display sensor data on the LCD.
Check for emergency conditions (Temperature, Sound, Distance, Air Quality).
3.1. Emergency Detected:
- Activate visual and audible alerts (LEDs, Buzzer).
- Display emergency message on the LCD.
- Log the emergency event.
- Send emergency email notification.
- Execute specific emergency actions based on the detected condition.
3.2. No Emergency:
- Display safe status indicators (LEDs, LCD).
- Display specific sensor data.
- Check if light intensity requires automatic lighting control.
Automatic Lighting Control:
If light intensity is low:
Turn on automatic lighting (Relay for lighting).
Display "Automatic Lighting: ON" on the LCD.
If light intensity is sufficient:
Turn off automatic lighting.
Display "Automatic Lighting: OFF" on the LCD.
Emergency Kits Location:
Display the location of emergency kits on the LCD.
User Interaction:
Provide information and feedback on the LCD.
Allow users to view sensor data, emergency history, etc.
Loop Iteration:
Repeat the loop at a specified interval (e.g., every second).
User Interaction (Button Press):
If the button is pressed:
Display "System Stopped" on the LCD.
Turn off LEDs, Buzzer, and automatic lighting.
Close communication channels.
Terminate the program.
</pre>

# Purpose of each sensor:
<pre>
LEDs (Red, Blue, Green):
Purpose: Visual indication of system status and emergency alerts.
Red LED: Indicates emergency conditions.
Blue LED: Indicates system activation and status.
Green LED: Indicates safe conditions.
</pre>

![image](https://github.com/Zakeer-official/Coal_Mine_Evacuation_System/assets/102544273/84752aa1-e284-43b2-bbfa-a1b197b89ebf)

<pre>
Sound Sensor:
Purpose: Detects unusual or loud noises that might indicate hazardous situations, such as collapses or machinery malfunctions.
</pre>   

![image](https://github.com/Zakeer-official/Coal_Mine_Evacuation_System/assets/102544273/a8377ee3-63b7-4574-9323-903c9a293fd0)

<pre>
Temperature and Humidity Sensor:
Purpose: Monitors the temperature and humidity levels in the mine to ensure optimal working conditions and to detect overheating or excessive moisture.
</pre>

![image](https://github.com/Zakeer-official/Coal_Mine_Evacuation_System/assets/102544273/9a62ce69-f916-4d79-ad3d-5a0ba9e5ffa2)


<pre>
Light Sensor:
Purpose: Measures ambient light intensity to adjust lighting controls and ensure optimal visibility for miners during evacuations.
</pre>

![image](https://github.com/Zakeer-official/Coal_Mine_Evacuation_System/assets/102544273/f067eefc-203a-4774-ac6d-3a2d7be6f945)


<pre>
Button:
Purpose: Initiates the activation of the system. Miners press the button to start the monitoring and emergency response functions.
</pre>

![image](https://github.com/Zakeer-official/Coal_Mine_Evacuation_System/assets/102544273/1c86c4c9-f183-45d1-ae79-49299debd58c)

<pre>
Ultrasonic Sensor:
 Purpose: Measures distances to detect obstacles or obstructions in the path, helping miners navigate safely.
</pre>

![image](https://github.com/Zakeer-official/Coal_Mine_Evacuation_System/assets/102544273/e000f1f1-6024-40ba-8e83-8b43f31d02b9)

<pre>
Rotary Angle Sensor:
Purpose: Measures the angle of rotation. It can be used for tasks like detecting the position of doors, hatches, or other movable objects.
</pre>

![image](https://github.com/Zakeer-official/Coal_Mine_Evacuation_System/assets/102544273/85e84019-d9ba-4835-933f-464808896fe6)

<pre>
Buzzer:
Purpose: Provides audible alerts and alarms during emergency situations to ensure miners are alerted even if they can't see visual indicators.
</pre>

![image](https://github.com/Zakeer-official/Coal_Mine_Evacuation_System/assets/102544273/e7d19692-d634-48f0-a142-2a9448b9dc4b)

<pre>
RGB LCD Display:
Purpose: Displays real-time sensor data, system status, emergency alerts, and any other relevant information for miners.
</pre>

![image](https://github.com/Zakeer-official/Coal_Mine_Evacuation_System/assets/102544273/00b7c3b0-fa15-44c9-9d22-8fc58045727f)

<pre>
Air Quality Sensor:
Purpose: Measures the air quality by detecting the presence of harmful gases, ensuring miners are not exposed to dangerous gas levels.
Relay (Optional for Automatic Lighting):
Purpose: Controls external devices like lights, enabling the system to automatically adjust lighting conditions based on the ambient light intensity.
</pre>

 ![image](https://github.com/Zakeer-official/Coal_Mine_Evacuation_System/assets/102544273/7bcfc752-3c1a-4642-8d76-0e220978db97)

Each sensor plays a crucial role in detecting potential hazards, communicating information to miners, and facilitating a prompt response during emergencies. Their collective integration forms a comprehensive system designed to enhance safety measures within coal mines.   

![image](https://github.com/Zakeer-official/Coal_Mine_Evacuation_System/assets/102544273/52302bdb-3204-4a46-9b46-2cf097055cb3)
                                                                                               
#Since time is not there we are not able to keep things properly instead we keep just kept which pin to keep where
<pre> 
LEDs (Red, Blue, Green):
Red LED: Connect to digital pin D5.
Blue LED: Connect to digital pin D6.
Green LED: Connect to digital pin D7.
Sound Sensor: Connect to analog pin A1.
Temperature and Humidity Sensor: Connect to digital pin D2.
Light Sensor: Connect to analog pin A0.
Button: Connect to digital pin D8.
Ultrasonic Sensor:
Connect the trigger pin to digital pin D3.
Connect the echo pin to digital pin D4.
Rotary Angle Sensor: Connect to analog pin A0.
Buzzer:
Connect to digital pin D4.
RGB LCD Display:
Connect the I2C SDA pin to the SDA pin on Grove Pi.
Connect the I2C SCL pin to the SCL pin on Grove Pi.
</pre>
Air Quality Sensor:
Connect to analog pin A1. 
 
# Conclusion:                                    
In the heart of coal mining's challenges, the "Coal Mine Evacuation System" emerges as a sentinel of safety. By fusing innovation and sensors, we've erected a fortress against danger, guiding miners through hazards with precision. This project isn't just about electronics; it's a testament to our commitment to human lives. As we close this chapter, the system's LEDs, alerts, and LCD fade, leaving a profound impact on safety standards. In the mine's depths, our creation echoes the harmonious blend of technology and empathy, underlining the future of safety protocols.

# Arduino-Automatic-Room-Lightening-System-
Automatic Room Lights System using Arduino is a very useful project as you need not worry about turning on and off the switches every time you want to turn on the lights. The main components of the Automatic Room Lights project are Arduino, PIR Sensor and the Relay Module.

Out of the three components, the PIR Sensor is the one in focus as it is the main device that helps in detecting humans and human motion.

In fact, the Automatic Room Lights project can be considered as one major application of the PIR Sensor. A similar concept is being already implemented in automatic toilet flush valves, hand dryers, etc.

# Working of the Project
The Automatic Room Lights using Arduino and PIR Sensor is a simple project, where the lights in the room will automatically turn on upon detecting a human motion and stay turned on until the person has left or there is no motion.

Working of this project is very simple and is explained here.

Initially, when there is no human movement, the PIR Sensor doesn’t detect any person and its OUT pin stays LOW. As the person enters the room, the change in infrared radiation in the room is detected by the PIR Sensor.

As a result, the output of the PIR Sensor becomes HIGH. Since the Data OUT of the PIR Sensor is connected to Digital Pin 8 of Arduino, whenever it becomes HIGH, Arduino will activate the relay by making the relay pin LOW (as the relay module is an active LOW module).

This will turn the Light ON. The light stays turned ON as long as there is movement in front of the sensor.

If the person takes a nap or leaves the room, the IR Radiation will become stable (there will be no change) and hence, the Data OUT of the PIR Sensor will become LOW. This in turn will make the Arduino to turn OFF the relay (make the relay pin HIGH) and the room light will be turned OFF.

# Visitor_Counter_Code

*The code is in the master branch*

Requirements:
1. STM32CubeIDE
2. STM32F103C6T6A Microcontroller
3. ST-Link V2

Debug Info:
1. Connect the Microcontroller to the PC using the bootloader.
2. Copy the master directory to the PC.
3. Open the directory in STM32CubIDE.
4. Click on the compile option and then debug button.
5. Before "while" block is the setup code.
6. The global variables (Sensor_0_activation, Sensor_1_activation, numInVis, numOutVis, timerActivate) tell us the state of the system.
7. System only waits 2sec for a person to be counted, if more than 2 sec are taken then earlier readings are discarded.
8. Step wise debugging can be done but the timer should be taken care of.
9. To input different scenarios the codes in the while block need to be put in the respective order.
10. "EXTI_LINE_SWI" is a function that generates software interrupt on the input line.
11. "SENSOR_0_PIN_NUM" is used to specify Pin 12 as Sensor 0 is connected to PA12.
12. "SENSOR_1_PIN_NUM" is used to specify Pin 7 as Sensor 1 is connected to PA7.
13. "timerActivate" tells us whether the timer is currenlty active or not. [1 == Active]


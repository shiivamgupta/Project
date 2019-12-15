Hi All,
Hope you have completed the UART Assignment

Now its time to use some new tools via demo of ADC
Goal: Setup ADC on STM and Display the Output on STM Studio

Hardware Required 1K Pot , Breadboard , Connecting Cables
Two Options and a Workaround

Option 1





Option 2






Workaround

For 8 bit ADC
i.Short ADCx Pin with VCC(3.3v) , Value that will get Displayed on STM Studio 255
ii.Short ADCx Pin with GND(0.0v) , Value that will get Displayed on STM Studio 0
Tips & Tricks for Using STM Studio
    1. STM Studio always displays Global Variables (Define the uint32_t adcval in //USER CODE BEGIN 0//)
    2. STM Studio doesn’t Works when the Board is in the Debug State in Keil.
How To Work on STM Studio and Keil Debug
https://youtu.be/DOxks_34RVk


Hi All,
Hope you have completed the ADC Assignment

 

Now it’s time to implement some core functionalities like SPI

Goal: Interacting with On-Board 3D Accelerometer via SPI bus and viewing the output on STM Studio or Keil

 

Hardware Required : NO Extra Hardware Required , 3D Acc. Is On Board itself (LIS3DSH MEMS digital output motion sensor: ultra-low-power high-performance three-axis "nano" accelerometer)

 

Two Options to Implement this

 

Option 1 : Using Polling Approach

 

Option 2 : Using Interrupts

 

Datasheet for 3D Acc. Is attached

 

Code Explanation:

1.  Need to Set Few Buffers so that we can transmit and receive data on SPI bus (uint8_t TxBuf[2],RxBuf_X[2],ReturnVal[2],RxBuf_Y[2],RxBuf_Z[2] ] in /* USER CODE BEGIN 0 */)
2.  SPI_Transmit(), SPI_Receive() will be the two API’s by which we will be sending the data
3.  The Data kept in the TxBuf will be the Register Information for 3D Acc. Example: TxBuf[0]=0x20(This is Control Register 4), TxBuf[1]=0x17(This is value we are sending to Control Register 4)
4. Images
5. Also Chip Select is done by HAL_GPIO_WritePin(portE, pin 3)

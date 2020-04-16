# STM32F429ZI_NUCLEO_144_AP_MODE
> Adding Embedded Wi-Fi Connectivity to a Cortex-M4 Microcontroller

This collection of sample applications demonstrate many Wi-Fi use cases using the Microchip WINC1500 Wi-Fi module connected to an STM32F429ZI Host MCU.

For more information on Microchip WINC1500 Wi-Fi Module, visit Microchip webpage: http://www.microchip.com/atwinc1500
For more information on STM32F249ZI MCU, visit ST webpage: https://www.st.com/en/microcontrollers/stm32f429zi.html

![](Doc/SETUP.png)

## Software

- Atollic TrueSTUDIO v9.3.0 has been used on Windows for this project. </br>
To download the IDE, visit http://www.atollic.com/truestudio/

- TeraTerm terminal emulator </br>
To download the program, visit https://ttssh2.osdn.jp/index.html.en


## Hardware Setup

STM32 Nucleo-144 development board with STM32F429ZI MCU
STM32 Nucleo-144 board does not require any debug probe as it integrates the ST-LINK/V2-1 debugger/programmer.</br>
The USB connector CN1 will be used to power supply the board, program the MCU and interact with the serial console.</br>
More information available:  https://www.st.com/en/evaluation-tools/nucleo-f429zi.html
![](Doc\NUCLEO-F429ZI.png)

The ATWINC1500-XPRO extension board allows you to evaluate the Microchip WINC1500 WiFi module.</br>
More information available: https://www.microchip.com/DevelopmentTools/ProductDetails/ATWINC1500-XPRO
![](Doc/WINC1500-XPRO.png)

![](Doc/WIRING.png)


## Tutorial

- Start Atollic TrueSTUDIO IDE
- Import an existing project
- Browse your hard disk to select the project folder of this sample code
- Open inc/main.h to change the AP credentials if required
- In AP mode, open main.c file to change the IP address of the AP if required
- Open TeraTerm program a create a serial connection with the following parameters: 115200bps, 8 bit, no parity, 1 stop bit
- Build project, if everything is set correctly build finishes without errors
- Open the Debug Configurations window and make sure ST-LINK is selected as a debug probe with SWD interface
- Start debug/program the code into your board
- Run the code
- You should now be able to see serial traces on the TeraTerm console


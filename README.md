## Adafruit GPS driver for STM32Fx

The driver has methods to send commands, retrieve and process messages coming from GPS sensor through UART. 
An example usage can be found in [/Src/main.cpp](/src/main.cpp). 

If you are using CubeMX, you are expected to enable UART2 and its interrupts to run the example code in *main.cpp*. 

*HAL_UART_RxCpltCallback* in the *main.cpp* receives information from the GPS sensor manipulates it using the driver
and prints the processed output.

In order printf to work properly, you need to follow the steps shared in this [link](http://www.keil.com/support/man/docs/uv4/uv4_db_dbg_printf_viewer.htm) 

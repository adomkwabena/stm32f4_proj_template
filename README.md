# STM32F4 Project Template
This is a project template for the STM32F4 discovery board. 
Instead of building a project from scratch, you can clone this project
and use it as a starting point. 

## Support
There is currently support for only the STM32F407VGT06 microcontroller, but
porting to other STM32F4 devices should be a breeze.

## Features
The project template supports these basic features

- I2C driver for the I2C1 peripheral
- SPI driver for the SPI1 peripheral
- UART drivers for the USART1 and USART2 peripherals

These peripheral drivers can be easily ported to other hardware instances.
This is because most of the instances retain the same registers.
For example the USART2 driver is a port of the USART1 driver. 

## Building and Programming
You can clone the project, rename it and start adding your own code.

To build run
```
cd stm32f4_project_template
make
```

To program the STM32F4 discovery board, run 
```
cd stm32f4_project_template
make burn
```

# alios-things_stm32f103rct6_hello
[WIP] The Alios Things hello MDK4 (Keil 4) project porting to zhongjingyuan stm32f103rct6 develop board

## Ref  
* based on 2.1.0  
https://github.com/alibaba/AliOS-Things/releases/tag/v2.1.0  

## MDK4 (Keil4) Project  
* see projects/helloworld.uvproj  
* see projects/readme.txt  

## Issues  
* USART2 (PA2 TX, PA3 RX) is OK, but USART1 is not OK (see vendor/stm32f103rct6.pdf)    
* In MDK4 emulator (Debug Session), please open UART2, not UART1  
* Some code in drivers/sensor/hal/sensor_hal.c is changed, see vendor/sensor_config.c and vendor/sensor_config.txt, sensor_config.c is generated by aos-cube, but not used here  

## Build original project (branch rel_2.1.0) with aos-cube  
* see vendor/alios_things_aos_build.txt  

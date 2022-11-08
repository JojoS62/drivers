add_library(bsp-DISCO_F769NI INTERFACE)

target_include_directories(bsp-DISCO_F769NI INTERFACE 
    BSP/STM32F769I-Discovery
    LCD_DISCO_F769NI
    TS_DISCO_F769NI
)

target_sources(bsp-DISCO_F769NI
    INTERFACE
        BSP/Components/adv7533/adv7533.c
        BSP/Components/ft6x06/ft6x06.c
        BSP/Components/otm8009a/otm8009a.c
        BSP/Components/wm8994/wm8994.c
        BSP/Components/nt35510/nt35510.c
        BSP/Fonts/font8.c
        BSP/Fonts/font12.c
        BSP/Fonts/font16.c
        BSP/Fonts/font20.c
        BSP/Fonts/font24.c
        BSP/STM32F769I-Discovery/stm32f769i_discovery_audio.c
        BSP/STM32F769I-Discovery/stm32f769i_discovery_eeprom.c
        BSP/STM32F769I-Discovery/stm32f769i_discovery_lcd.c
        BSP/STM32F769I-Discovery/stm32f769i_discovery_qspi.c
        BSP/STM32F769I-Discovery/stm32f769i_discovery_sdram.c
        BSP/STM32F769I-Discovery/stm32f769i_discovery_ts.c
        BSP/STM32F769I-Discovery/stm32f769i_discovery.c
        LCD_DISCO_F769NI/LCD_DISCO_F769NI.cpp
        TS_DISCO_F769NI/TS_DISCO_F769NI.cpp
)


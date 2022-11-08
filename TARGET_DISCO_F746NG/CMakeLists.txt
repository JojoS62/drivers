add_library(bsp-DISCO_F746NG INTERFACE)

target_include_directories(bsp-DISCO_F746NG INTERFACE 
    BSP/STM32F746G-Discovery
    LCD_DISCO_F746NG
    TS_DISCO_F746NG
)

target_sources(bsp-DISCO_F746NG
    INTERFACE
        BSP/Components/ft5336/ft5336.c
        BSP/Fonts/font8.c
        BSP/Fonts/font12.c
        BSP/Fonts/font16.c
        BSP/Fonts/font20.c
        BSP/Fonts/font24.c
        BSP/STM32F746G-Discovery/stm32746g_discovery_audio.c
        BSP/STM32F746G-Discovery/stm32746g_discovery_eeprom.c
        BSP/STM32F746G-Discovery/stm32746g_discovery_lcd.c
        BSP/STM32F746G-Discovery/stm32746g_discovery_qspi.c
        BSP/STM32F746G-Discovery/stm32746g_discovery_sdram.c
        BSP/STM32F746G-Discovery/stm32746g_discovery_ts.c
        BSP/STM32F746G-Discovery/stm32746g_discovery.c
        LCD_DISCO_F746NG/LCD_DISCO_F746NG.cpp
        TS_DISCO_F746NG/TS_DISCO_F746NG.cpp
)


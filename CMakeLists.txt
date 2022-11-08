add_library(bsp INTERFACE)

if("DISCO_F769NI" IN_LIST MBED_TARGET_LABELS)
    add_subdirectory(TARGET_DISCO_F769NI)
    target_link_libraries(bsp INTERFACE bsp-DISCO_F769NI)
endif()

if("DISCO_F746NG" IN_LIST MBED_TARGET_LABELS)
    add_subdirectory(TARGET_DISCO_F746NG)
    target_link_libraries(bsp INTERFACE bsp-DISCO_F746NG)
endif()

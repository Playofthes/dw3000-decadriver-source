idf_component_register(
    SRCS
        "dwt_uwb_driver/src/dw3000_device.c"
        "platform/esp-idf/dw3000_hw.c"
        "platform/esp-idf/dw3000_spi.c"
    INCLUDE_DIRS
        "dwt_uwb_driver/inc"
        "platform/esp-idf"
    REQUIRES
        driver esp_driver_spi esp_driver_gpio esp_timer freertos
)
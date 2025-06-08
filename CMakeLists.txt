project( synthesize_audio_ac)

# Cria o executável com os arquivos-fonte
add_executable(${PROJECT_NAME}
        main.c
        i2c_setup.c
        oled_setup.c
        ssd1306.c
        rgb_setup.c
        capture_audio_setup.c
        audio_playback.c
        buttons_setup.c
        )

# Diretórios de inclusão
target_include_directories(${PROJECT_NAME}
        PUBLIC
        ${CMAKE_CURRENT_SOURCE_DIR}/include
        )

# Vincula bibliotecas necessárias
target_link_libraries(${PROJECT_NAME}
        pico_stdlib
        hardware_adc
        hardware_i2c
        hardware_dma
        hardware_pwm
        hardware_gpio
        )

pico_add_extra_outputs(${PROJECT_NAME})

example_auto_set_url(${PROJECT_NAME})

pico_enable_stdio_usb(${PROJECT_NAME} 1)

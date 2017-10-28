cmake_minimum_required(VERSION 3.8)
project(lcd_game)

set(CMAKE_CXX_STANDARD 11)

set(SOURCE_FILES
        pre_emptive_os/api/general.h
        pre_emptive_os/api/osapi.h
        pre_emptive_os/core/_oshal/api/a7hal.h
        pre_emptive_os/core/_oshal/api/general.h
        pre_emptive_os/core/_oshal/stub/oshalstub.h
        pre_emptive_os/core/count_sem.h
        pre_emptive_os/core/error.h
        pre_emptive_os/core/event.h
        pre_emptive_os/core/hal.h
        pre_emptive_os/core/kernel.h
        pre_emptive_os/core/pcb.h
        pre_emptive_os/core/prioqueue.h
        pre_emptive_os/core/queue.h
        pre_emptive_os/core/stack_usage.h
        pre_emptive_os/core/timer.h
        pre_emptive_os/stub/osstub.h
        startup/config.h
        startup/consol.c
        startup/consol.h
        startup/ea_init.h
        startup/framework.c
        startup/framework.h
        startup/general.h
        startup/lpc2xxx.h
        startup/printf_P.h
        adc.c
        adc.h
        ascii.h
        eeprom.c
        eeprom.h
        i2c.c
        i2c.h
        key.c
        key.h
        lcd.c
        lcd.h
        lcd_hw.c
        lcd_hw.h
        main.c
        pca9532.c
        pca9532.h
        select.c
        select.h
        snake.c
        snake.h)

add_executable(lcd_game ${SOURCE_FILES})
# SPDX-License-Identifier: Apache-2.0
cmake_minimum_required(VERSION 3.26)
set(BOARD blackpill_f401cc)
#set(DTC_OVERLAY_FILE "${CMAKE_CURRENT_SOURCE_DIR}/boards/stm32f401.overlay")
#set(DTC_OVERLAY_FILE "boards/blackpill_f401cc.overlay")
find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})

project(NONE)

target_sources(app PRIVATE
        src/main.c
)

# Other board-specific configuration options can go here

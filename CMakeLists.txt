cmake_minimum_required(VERSION 3.20.0)

# list(APPEND BOARD_ROOT ${CMAKE_CURRENT_SOURCE_DIR})
# message(FATAL_ERROR ${BOARD_ROOT})

find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})

project(flight_logger LANGUAGES C)


target_sources(app PRIVATE src/main.c)



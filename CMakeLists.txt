cmake_minimum_required(VERSION 3.2)
project(firmatac)

set(SOURCE_FILES
    includes/firmata.h
    includes/serial.h
    includes/servo.h
    src/firmata.c
    src/serial.c
    src/servo.c
)

include_directories(
    .
    includes
)

add_library(firmatac SHARED ${SOURCE_FILES})
set_target_properties(
    firmatac PROPERTIES LINKER_LANGUAGE C
)


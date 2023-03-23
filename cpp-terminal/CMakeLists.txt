cmake_minimum_required(VERSION 3.5)

project(kilo-editor LANGUAGES C)

add_executable(kilo-editor kilo.c)
set_property(TARGET kilo-editor PROPERTY C_STANDARD 99)

install(TARGETS kilo-editor
    LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR})

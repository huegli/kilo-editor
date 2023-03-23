cmake_minimum_required(VERSION 3.25)
project(kilo-cppt)

set(CMAKE_CXX_STANDARD 23)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

include_directories(cpp-terminal)

add_subdirectory(cpp-terminal)
add_executable(${PROJECT_NAME} main.cpp )
target_link_libraries(kilo PRIVATE cpp-terminal::cpp-terminal Warnings::Warnings)

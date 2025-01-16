# Specify minimum CMake version
cmake_minimum_required(VERSION 3.5)

# Project name and language
project(HelloWin32 LANGUAGES C)

# Add executable with WIN32 subsystem
add_executable(HelloWin32 WIN32 hello.c)

# Link required Windows libraries
target_link_libraries(HelloWin32 PRIVATE user32)

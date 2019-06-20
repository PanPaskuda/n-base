# Specify the minimum version for CMake

cmake_minimum_required(VERSION 3.5)

# Project's name

project(N-Base)
# Set the output folder where your program will be created
set(CMAKE_BINARY_DIR ${CMAKE_SOURCE_DIR}/bin)
set(EXECUTABLE_OUTPUT_PATH ${CMAKE_BINARY_DIR})
set(LIBRARY_OUTPUT_PATH ${CMAKE_BINARY_DIR})

# The following folder will be included
include_directories("${PROJECT_SOURCE_DIR}")

# Files to compile
add_executable(hello ${PROJECT_SOURCE_DIR}/application/main.c)

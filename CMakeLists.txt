cmake_minimum_required(VERSION 3.10)

project(CrossArrayProject CXX)

# Set C++ standard
cmake_policy(SET CMP0015 NEW)
set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Include directories
include_directories(src)

# Source files
set(SOURCES
    src/CrossArray.cpp
)

# Create executable
add_executable(code ${SOURCES})

# Compiler options
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -O2 -Wall -Wextra -Werror")

cmake_minimum_required(VERSION 3.10)
project(linkedlist LANGUAGES CXX)

# Set C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Add include directory
include_directories(${CMAKE_SOURCE_DIR}/include)

# Collect all source files
file(GLOB SRC_FILES ${CMAKE_SOURCE_DIR}/src/*.cpp)

# Create executable
add_executable(${PROJECT_NAME} ${SRC_FILES})
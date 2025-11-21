cmake_minimum_required(VERSION 3.10)

project(liblinkedlist LANGUAGES CXX)

add_subdirectory(tools)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_library(linkedlist INTERFACE)
target_include_directories(linkedlist INTERFACE
${CMAKE_CURRENT_SOURCE_DIR}/include
)
target_link_libraries(linkedlist INTERFACE tools)

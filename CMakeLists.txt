project(sp_lab4)
cmake_minimum_required(VERSION 3.2)


set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/res)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/res)
set(CMAKE_GENERATOR "Ninja")
add_library(libFile SHARED calculator.cpp)
add_executable(script main.cpp)
target_link_libraries(script libFile)

cmake_minimum_required(VERSION 3.10)
project(CalculatorProject)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

add_library(calculator STATIC calculator.cpp)

add_executable(calculator_app main.cpp)

target_link_libraries(calculator_app PRIVATE calculator)

# cmake_minimum_required(VERSION <specify CMake version here>)
cmake_minimum_required(VERSION 3.6)

add_definitions(-std=c++11)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -Wall -Ofast -Wfatal-errors -D_MWAITXINTRIN_H_INCLUDED")

include_directories(${PROJECT_SOURCE_DIR}/include)

add_library(source)

add_definitions(-O2 -pthread)
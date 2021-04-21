# cmake_minimum_required(VERSION <specify CMake version here>)
cmake_minimum_required (VERSION 3.6)

add_definitions(-std=c++11)
set(CMAKE_CXX_STANDARD 11)

project(CSRIWebServer)

include_directories(${PROJECT_SOURCE_DIR}/include)

# 包含子项目。
add_subdirectory (src)

add_executable(CSRIWebServer main.cpp)


add_definitions(-O2 -pthread)
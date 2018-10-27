#Project name
project(HybridAStar)

#Version
cmake_minimum_required (VERSION 3.5)
add_definitions(-std=c++11)

#Enable warnings
set(CXX_FLAGS "-Wall")
set(CMAKE_CXX_FLAGS "${CXX_FLAGS}")

#src files
file(GLOB sources "src/*.cpp")

#header files
include_directories(include)

#Destination file
add_executable(hybridAStar ${sources})
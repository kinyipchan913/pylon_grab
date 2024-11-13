cmake_minimum_required(VERSION 3.9)
project (grab)

# Locate pylon.
find_package(pylon 7.2.1 REQUIRED)
# Find OpenCV package
find_package(OpenCV REQUIRED)

# Include directories from OpenCV
include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(grab Grab.cpp)

target_link_libraries(grab pylon::pylon)
# Link OpenCV libraries
target_link_libraries(grab ${OpenCV_LIBS})
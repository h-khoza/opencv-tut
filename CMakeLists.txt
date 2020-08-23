cmake_minimum_required(VERSION 3.0)
project(openCVProject)

set(CMAKE_BUILD_TYPE Debug)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++14")

find_package(OpenCV REQUIRED)

add_executable(
  openCVProject
  src/main.cpp
  )

target_link_libraries(openCVProject ${OpenCV_LIBS})
 

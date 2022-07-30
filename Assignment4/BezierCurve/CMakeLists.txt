cmake_minimum_required(VERSION 3.22)
project(BezierCurve)

set(CMAKE_CXX_STANDARD 17)

find_package(OpenCV REQUIRED)
include_directories("/opt/homebrew/Cellar/opencv/4.5.5_3/include")

add_executable(BezierCurve main.cpp)
target_link_libraries(BezierCurve ${OpenCV_LIBRARIES})



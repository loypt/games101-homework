cmake_minimum_required(VERSION 3.22)
project(Rasterizer)

set(CMAKE_CXX_STANDARD 17)

find_package(Eigen3 REQUIRED)
include_directories("/opt/homebrew/Cellar/eigen/3.4.0_1/include")

find_package(OpenCV REQUIRED)
include_directories("/opt/homebrew/Cellar/opencv/4.5.5_3/include")

add_executable(Rasterizer main.cpp rasterizer.cpp rasterizer.h Triangle.cpp Triangle.h global.h)
target_link_libraries(Rasterizer ${OpenCV_LIBRARIES})

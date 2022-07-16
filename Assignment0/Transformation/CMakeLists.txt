cmake_minimum_required(VERSION 3.22)
project(Transformation)

set(CMAKE_CXX_STANDARD 14)

find_package(Eigen3 REQUIRED)
include_directories("/opt/homebrew/Cellar/eigen/3.4.0_1/include")

add_executable(Transformation main.cpp)

cmake_minimum_required(VERSION 3.31)

project(kalman VERSION 0.1)

# Find OpenCV
find_package(OpenCV 4.11 REQUIRED core)


add_executable(kalman kalman.cpp)
target_link_libraries(kalman opencv_core opencv_highgui opencv_video)
cmake_minimum_required(VERSION 3.12)
project(Test)

set(CMAKE_CXX_STANDARD 14)
set(OpenCV_DIR %OPENCV_DIR%)
find_package(OpenCV REQUIRED)

add_executable(Test main.cpp penis.cpp penis.h)

include_directories(${OpenCV_INCLUDE_DIRS})
target_link_libraries(Test ${OpenCV_LIBS})
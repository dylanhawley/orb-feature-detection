cmake_minimum_required(VERSION 2.8)
set(CMAKE_CXX_STANDARD 11)
project( detect_features )
find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )
add_executable( detect_features main.cpp )
target_link_libraries( detect_features ${OpenCV_LIBS} )
cmake_minimum_required(VERSION 3.17)
project(opencv_cmake_template)
find_package(OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )
set(CMAKE_CXX_STANDARD 17)

add_executable( main main.cc )
target_link_libraries( main ${OpenCV_LIBS} )

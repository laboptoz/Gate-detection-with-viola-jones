# Declare the version of the CMake API for forward-compatibility
cmake_minimum_required(VERSION 2.8)

project(corner_detect_haarcascades)

#set( OpenCV_FOUND 1 )
#set( OpenCV_DIR "/usr/share/OpenCV/" )
find_package( OpenCV REQUIRED )

add_executable (corner_detect_haarcascades ${PROJECT_SOURCE_DIR}/src/corner_detect_haarcascades.cpp)

target_link_libraries( corner_detect_haarcascades ${OpenCV_LIBS} )


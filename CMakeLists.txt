cmake_minimum_required(VERSION 2.8)
project(RM_code4)
SET(CMAKE_BUILD_TYPE Release)
#set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)
#set(LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/lib)
#include_directories(${PROJECT_SOURCE_DIR}/include)
find_package( OpenCV REQUIRED )
add_executable(test1 src/layer.cpp src/main.cpp src/network.cpp )
target_link_libraries( test1 ${OpenCV_LIBS} )

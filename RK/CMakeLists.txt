cmake_minimum_required(VERSION 3.10)
project(rk VERSION 0.1)
include(ctest)

set(CMAKE_CXX_STANDARD 14)
set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/build/bin)
include_directories(${PROJECT_NAME} ${PROJECT_SOURCE_DIR}/inc/${PROJECT_NAME})
add_subdirectory(libs)
add_subdirectory(src)
add_subdirectory(test)

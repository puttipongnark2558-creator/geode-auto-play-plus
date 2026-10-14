cmake_minimum_required(VERSION 3.13)
set(CMAKE_CXX_STANDARD 20)

include($ENV{GEODE_SDK}/cmake/GeodeFile.cmake)
project(AutoPlayPlus)

file(GLOB_RECURSE SOURCES "src/*.cpp" "src/*.hpp")

add_library(${PROJECT_NAME} SHARED ${SOURCES})

setup_geode_mod(${PROJECT_NAME})

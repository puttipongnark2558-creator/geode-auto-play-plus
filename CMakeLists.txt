cmake_minimum_required(VERSION 3.13)
set(CMAKE_CXX_STANDARD 20)

include($ENV{GEODE_SDK}/cmake/GeodeFile.cmake)
project(AutoPlayPlus)

setup_geode_mod(AutoPlayPlus)

add_subdirectory(src)

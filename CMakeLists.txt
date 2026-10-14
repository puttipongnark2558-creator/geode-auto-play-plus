cmake_minimum_required(VERSION 3.13)
set(CMAKE_CXX_STANDARD 20)

include($ENV{GEODE_SDK}/cmake/GeodeFile.cmake)
project(AutoPlayPlus)

# 1. Add src sub-directory FIRST so add_geode_mod creates the target
add_subdirectory(src)

# 2. Setup the geode mod target AFTER it exists
setup_geode_mod(AutoPlayPlus)

cmake_minimum_required(VERSION 3.14)

project(lecture_8_live C)

set(CMAKE_C_STANDARD 11)

# Include dependencies
include(rps/cmake/mtest.cmake)

add_subdirectory(src)
enable_testing()
add_subdirectory(test)

# A full rock-paper-scissor program and test is in the 'rps' folder.
add_subdirectory(rps)

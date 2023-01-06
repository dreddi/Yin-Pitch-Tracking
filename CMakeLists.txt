cmake_minimum_required(VERSION 3.6)

project(yin-pitch-tracking)

add_library(libyin Yin.c)
target_include_directories(libyin INTERFACE .)

add_executable(test_yin Test_Yin.c)
target_link_libraries(test_yin libyin)


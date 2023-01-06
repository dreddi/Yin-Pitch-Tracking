cmake_minimum_required(VERSION 3.6)

project(yin-pitch-tracking)

add_library(yin STATIC Yin.c)
target_include_directories(yin INTERFACE .)

add_executable(test_yin Test_Yin.c)
target_link_libraries(test_yin yin)


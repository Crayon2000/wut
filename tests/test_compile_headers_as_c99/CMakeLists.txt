cmake_minimum_required(VERSION 3.2)
project(test_compile_headers_as_c99 C)
include("${DEVKITPRO}/wut/share/wut.cmake" REQUIRED)

set(CMAKE_C_STANDARD 99)

add_executable(test_compile_headers_as_c99
   main.c)

wut_create_rpx(test_compile_headers_as_c99)

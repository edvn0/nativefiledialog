cmake_minimum_required(VERSION 3.21)
project(nfd)

add_library(nfd STATIC src/common.h src/nfd_cocoa.m src/nfd_common.c src/simple_exec.h)

target_link_libraries(nfd PRIVATE "-framework AppKit")
target_include_directories(nfd PRIVATE src/include)

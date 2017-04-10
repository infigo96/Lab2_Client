cmake_minimum_required(VERSION 3.6)
project(Client)

set(CMAKE_C_STANDARD 99)

set(SOURCE_FILES main.c)
FIND_PACKAGE (Threads)
add_executable(Client ${SOURCE_FILES})
target_link_libraries( Client ${CMAKE_THREAD_LIBS_INIT} )
cmake_minimum_required(VERSION 3.7)
project(fib)

set(CMAKE_CXX_STANDARD 14)

# added -fopenmp
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -fopenmp")

set(SOURCE_FILES stream_fibo.c stream_recursive_fibo.c sync.h common.h fibo.c common.c)
add_executable(fib ${SOURCE_FILES})
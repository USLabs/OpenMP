cmake_minimum_required(VERSION 3.7)
project(OpenMP)

set(CMAKE_CXX_STANDARD 14)

# added -fopenmp
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -fopenmp")

set(SOURCE_FILES mergesort.c common.h common.c sync.h mergesort.h stream_df_mergesort.c)
add_executable(OpenMP ${SOURCE_FILES})
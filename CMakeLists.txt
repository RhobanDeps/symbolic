cmake_minimum_required(VERSION 2.8)

set (CMAKE_CXX_FLAGS "-std=c++11 -Wall -Wno-reorder -pedantic -fno-elide-constructors")

add_library(symbolic SHARED symbolicc++.cpp)
include_directories(${CMAKE_SOURCE_DIR})
set_target_properties(symbolic PROPERTIES COMPILE_DEFINITIONS "LIBSYMBOLICCPLUSPLUS")

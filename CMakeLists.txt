cmake_minimum_required(VERSION 2.8)

add_library(symbolic SHARED symbolicc++.cpp)
include_directories(${CMAKE_SOURCE_DIR})
set_target_properties(symbolic PROPERTIES COMPILE_DEFINITIONS "LIBSYMBOLICCPLUSPLUS")

cmake_minimum_required(VERSION 2.8 FATAL_ERROR)

set(PROJECT_NAME cpp_lib_skeleton)

project(${PROJECT_NAME})

set(CMAKE_CXX_FLAGS "-g -Wall")

include_directories(include)

set(SOURCE_FILES
	include/example.h
	src/example.cc
)

add_library(cpp_lib_skeleton ${SOURCE_FILES})
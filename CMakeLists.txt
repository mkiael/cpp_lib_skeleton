cmake_minimum_required(VERSION 2.8 FATAL_ERROR)

set(PROJECT_NAME cpp_lib_skeleton)

project(${PROJECT_NAME})

set(LIBRARY_NAME cpp_lib_skeleton)

set(CMAKE_CXX_FLAGS "-g -Wall")


set(SOURCE_FILES
	include/cpp_lib_skeleton/example.h
	src/example.cc
)

add_library(cpp_lib_skeleton ${SOURCE_FILES})

target_include_directories(${LIBRARY_NAME} PUBLIC
    $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
    $<INSTALL_INTERFACE:include>
)
cmake_minimum_required(VERSION 3.15)

project(Tclap
		LANGUAGES CXX
		DESCRIPTION "Provides TCLAP library as a CMake INTERFACE target"
		VERSION 1.2.2)

add_library(${PROJECT_NAME} INTERFACE)

target_include_directories(${PROJECT_NAME} INTERFACE ${CMAKE_CURRENT_SOURCE_DIR})

# Templatized C++ Command Line Parser Library (TCLAP)

This repository contains the TCLAP library from [http://tclap.sourceforge.net/](http://tclap.sourceforge.net/).

It can be downloaded from https://sourceforge.net/projects/tclap/

The repository contains a CMakeLists.txt file that adds this library as an interface target.

## Usage

To include this library in your project, assuming this repository is contained in `externalLibs/tclap`, adjust your main CMakeLists.txt file as below
Adjust your CMakeLists.txt similar to this example:
```
cmake_minimum_required(VERSION 3.15.0)

project(my_incredible_project LANGUAGES CXX)

add_subdirectory(externalLibs/tclap)

add_executable(
    ${PROJECT_NAME}
    main.cpp
)

set_target_properties(${PROJECT_NAME} PROPERTIES CXX_STANDARD 11)

target_compile_features(${PROJECT_NAME} PUBLIC cxx_std_11)

target_link_libraries(
    ${PROJECT_NAME}
    Tclap
)
```

# Usage

For usage of the library, please read the manual and exmaples at http://tclap.sourceforge.net/

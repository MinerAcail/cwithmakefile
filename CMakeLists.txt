cmake_minimum_required(VERSION 3.15)
project(CwithCmake)


add_subdirectory(include)
add_subdirectory(src)

option(BUILD_EXAMPLES "whether or not to build examples" ON)

if(BUILD_EXAMPLES)
    message(STATUS "Building examples...  ")
    add_subdirectory(example)
    
endif()
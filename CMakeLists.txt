cmake_minimum_required(VERSION 3.18)

project(tinyxml LANGUAGES CXX)

add_definitions(-DTIXML_USE_STL)
add_library(tinyxml STATIC tinyxml.cpp tinyxmlerror.cpp tinyxmlparser.cpp)
target_include_directories(tinyxml PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

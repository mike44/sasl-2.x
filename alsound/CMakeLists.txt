cmake_minimum_required(VERSION 2.8)

project(sasl-alsound)

file(GLOB_RECURSE SOURCES *.cpp)
file(GLOB_RECURSE HEADERS *.h)

include_directories(${SASL_INCL_DIRS} "../libavionics")

add_library(sasl-alsound STATIC ${SOURCES})

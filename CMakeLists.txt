cmake_minimum_required(VERSION 2.6.0)
project(poly2tri)

set(SRCS poly2tri/common/shapes.cc
        poly2tri/sweep/advancing_front.cc
        poly2tri/sweep/cdt.cc
        poly2tri/sweep/sweep.cc
        poly2tri/sweep/sweep_context.cc)

set( POLY2TRI_INCLUDE_DIR ${CMAKE_SOURCE_DIR}/poly2tri)
add_library(poly2tri ${SRCS})
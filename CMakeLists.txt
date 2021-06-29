# CMakeList.txt : CMake project for Geometry, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

project(Geometrylib VERSION 1.0.1 DESCRIPTION "Geometrylib description")

# Add source to this project's executable.
add_library (Geometrylib STATIC Geometry.cpp)
set_target_properties(Geometrylib PROPERTIES
    VERSION ${PROJECT_VERSION}
    SOVERSION 1
    PUBLIC_HEADER Geometry.h)

# TODO: Add tests and install targets if needed.

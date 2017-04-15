cmake_minimum_required(VERSION 2.8)

project(pathtracer)

# The version number
set (VERSION_MAJOR 0)
set (VERSION_MINOR 0)
set (VERSION_PATCH 0)
set (VERSION "${VERSION_MAJOR}.${VERSION_MINOR}.${VERSION_PATCH}")

# Include directories
include_directories("${PROJECT_SOURCE_DIR}/source")

# Include sources
file(GLOB SOURCES "source/**/*.cpp")

# Executables
add_executable(${PROJECT_NAME} ${SOURCES})

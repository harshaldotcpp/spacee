
# Minimum required CMake version
cmake_minimum_required(VERSION 3.22.0)

# Project name and language
project(spacee LANGUAGES CXX)

# Set output directory for libraries
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/lib)
include_directories(src/include)

# Define source files
set(SOURCE_FILES src/spacee.cpp)

# Create static library from source files
add_library(${PROJECT_NAME} STATIC ${SOURCE_FILES})

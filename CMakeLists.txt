cmake_minimum_required(VERSION 3.7.2)

project (hello)

# Set where the various files will be copied to within the build directory
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/lib)
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/lib/static)

# Set the directory where all header files are located
include_directories(${PROJECT_SOURCE_DIR}/include)

add_subdirectory(src)


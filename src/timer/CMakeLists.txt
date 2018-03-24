include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup(NO_OUTPUT_DIRS)

add_executable(timer timer.cpp)
target_link_libraries(timer ${CONAN_LIBS})


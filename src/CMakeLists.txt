add_library(add SHARED add.cpp)
#add_library(add STATIC add.cpp)
set_target_properties(add PROPERTIES VERSION 1.2.3 SOVERSION 1)
add_executable(hello helloworld.cpp)

target_compile_options(hello PUBLIC -std=c++0x -Wall -pedantic -Werror -Wextra)
target_link_libraries(hello add)

install(TARGETS hello DESTINATION bin)
install(TARGETS add DESTINATION lib)


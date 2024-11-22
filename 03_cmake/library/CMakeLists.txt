cmake_minimum_required(VERSION 3.17)
project(mySuperProject C)

set(CMAKE_C_STANDARD 99)

set(SOURCE main.c)
set(SOURCE_LIB lib/foo.c)

add_library(lib STATIC ${SOURCE_LIB})
add_executable(mySuperProject ${SOURCE})
target_link_libraries(mySuperProject lib)

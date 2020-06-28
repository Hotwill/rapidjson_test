cmake_minimum_required(VERSION 3.16)
project(rapidjson_test)

set(CMAKE_CXX_STANDARD 11)

include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup()

add_executable(rapidjson_test main.cpp)
target_link_libraries(rapidjson_test ${CONAN_LIBS})
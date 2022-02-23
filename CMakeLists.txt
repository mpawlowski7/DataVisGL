cmake_minimum_required(VERSION 3.21)
project(DataVisGL)

set(CMAKE_CXX_STANDARD 14)

include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup()

add_executable(DataVisGL main.cpp)
target_link_libraries(DataVisGL ${CONAN_LIBS})

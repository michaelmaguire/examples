cmake_minimum_required(VERSION 2.8.12)
project(PackageTest CXX)

set(CMAKE_PREFIX_PATH ${CMAKE_BINARY_DIR})
set(CMAKE_MODULE_PATH ${CMAKE_BINARY_DIR})

find_package(bye CONFIG)
add_executable(example example.cpp)
target_link_libraries(example bye::bye)

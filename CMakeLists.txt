cmake_minimum_required(VERSION 3.0 FATAL_ERROR)
project(recipe-01 LANGUAGES CXX)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -g")

add_executable(hello-world http_conn.cpp main.cpp)
target_link_libraries(hello-world pthread)

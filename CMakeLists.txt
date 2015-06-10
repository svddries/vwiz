cmake_minimum_required(VERSION 2.8.3)
project(wviz)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

include_directories(
    include
    3rdparty
)

add_executable(wviz src/wviz.cpp)
target_link_libraries(wviz boost_system)

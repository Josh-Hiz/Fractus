cmake_minimum_required(VERSION 3.31)
project(Fractus__)

set(CMAKE_CXX_STANDARD 20)

add_executable(Fractus__ src/main.cpp
        src/engine.cpp
        include/engine.h
        include/complex.h
)

find_package(SDL3 CONFIG REQUIRED)
target_link_libraries(Fractus__ PRIVATE SDL3::SDL3)

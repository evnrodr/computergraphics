cmake_minimum_required(VERSION 3.16)
project(computergraphics)

set(CMAKE_CXX_STANDARD 17)

add_executable(computergraphics src/main.cpp)
target_link_libraries(computergraphics -lglut -lglfw -lGLEW -lGL -lGLU)
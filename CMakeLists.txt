cmake_minimum_required(VERSION 3.16)
project(computergraphics)

set(CMAKE_CXX_STANDARD 17)

add_executable(computergraphics src/main.cpp src/Renderer.h src/Renderer.cpp src/VertexBuffer.h src/VertexBuffer.cpp src/IndexBuffer.h src/IndexBuffer.cpp src/VertexArray.cpp src/VertexArray.h src/VertexBufferLayout.cpp src/VertexBufferLayout.h)
target_link_libraries(computergraphics -lglut -lglfw -lGLEW -lGL -lGLU)
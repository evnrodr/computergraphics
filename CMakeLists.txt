cmake_minimum_required(VERSION 3.16)
project(computergraphics)

set(CMAKE_CXX_STANDARD 17)

add_executable(computergraphics src/Application.cpp src/Renderer.h src/Renderer.cpp src/VertexBuffer.h src/VertexBuffer.cpp src/IndexBuffer.h src/IndexBuffer.cpp src/VertexArray.cpp src/VertexArray.h src/VertexBufferLayout.cpp src/VertexBufferLayout.h src/Shader.cpp src/Shader.h src/vendor/stb_image/stb_image.h src/vendor/stb_image/stb_image.cpp src/Texture.cpp src/Texture.h src/vendor/imgui/imconfig.h src/vendor/imgui/imgui.cpp src/vendor/imgui/imgui.h src/vendor/imgui/imgui_demo.cpp src/vendor/imgui/imgui_draw.cpp src/vendor/imgui/imgui_impl_glfw_gl3.cpp src/vendor/imgui/imgui_impl_glfw_gl3.h src/vendor/imgui/imgui_internal.h src/vendor/imgui/stb_rect_pack.h src/vendor/imgui/stb_textedit.h src/vendor/imgui/stb_truetype.h)
include_directories(src/vendor)
target_link_libraries(computergraphics -lglut -lglfw -lGLEW -lGL -lGLU)
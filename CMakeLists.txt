cmake_minimum_required(VERSION 3.15)
project(learn_opengl CXX)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

find_package(glfw3 REQUIRED)
find_package(GLEW REQUIRED)

add_subdirectory(src/ep02)
add_subdirectory(src/ep03)
add_subdirectory(src/ep04-vertex-buffers)
add_subdirectory(src/ep05-vertex-attributes)
add_subdirectory(src/ep07-writing-shaders)
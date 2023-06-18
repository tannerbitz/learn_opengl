cmake_minimum_required(VERSION 3.15)
project(learn_opengl CXX)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

find_package(glfw3 REQUIRED)

add_subdirectory(src/ep02)

cmake_minimum_required(VERSION 3.15)
project(learn_opengl CXX)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

find_package(glfw3 REQUIRED)


add_executable(learn_opengl
    src/main.cpp
)

target_link_libraries(learn_opengl
    glfw
)


install(TARGETS learn_opengl DESTINATION "."
        RUNTIME DESTINATION bin
        ARCHIVE DESTINATION lib
        LIBRARY DESTINATION lib
        )

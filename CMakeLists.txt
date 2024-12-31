cmake_minimum_required(VERSION 3.15)
project(Simple2DGameEnginePractice)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED 20)
set(CMAKE_CXX_FLAGS "-Oz -ansi -Wall -Wextra")
set(CMAKE_CXX_FLAGS_DEBUG "-g -Wall -Wextra")

set(VERSION_MAJOR 0)
set(VERSION_MINOR 0)
set(VERSION_REVISION 0)

# Define executable
add_executable(Simple2DGameEngine
        src/main.cpp
)

target_link_libraries(Simple2DGameEngine
        GL
        GLFW
        GLEW
)
cmake_minimum_required(VERSION 3.0)
project(HelloWorldProject)

# Set the C++ standard to C++11 (you can adjust this if needed)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Enable compile_commands.json generation
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

# Include directories
include_directories(${PROJECT_SOURCE_DIR}/lib)

# Add the executable target
add_executable(hello_world
    app/main.cpp
    lib/hello_world.cpp
)

# Link pthread library
target_link_libraries(hello_world pthread)

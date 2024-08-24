cmake_minimum_required(VERSION 3.10)

# Set the project name and version
project(Pong VERSION 1.0)

# Specify the C++ standard
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

if(NOT CMAKE_BUILD_TYPE)
  set(CMAKE_BUILD_TYPE Debug)
endif()

# Add the executable
add_executable(Pong main.cpp Bat.cpp Bat.h)


find_package(SFML COMPONENTS system window graphics CONFIG REQUIRED)
target_link_libraries(Pong PRIVATE sfml-system sfml-network sfml-graphics sfml-window sfml-audio)

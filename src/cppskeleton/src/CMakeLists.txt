cmake_minimum_required(VERSION 3.20)

# Set the project name
project(cpp-skeleton)

# Add a library with the above sources
add_library(
    ${PROJECT_NAME}
    cppskeleton.cpp
)

target_include_directories(
    ${PROJECT_NAME} PUBLIC ./
)
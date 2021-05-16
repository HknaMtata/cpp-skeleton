cmake_minimum_required(VERSION 3.16)

add_subdirectory(src)

project(app)

add_executable(
    ${PROJECT_NAME}
    main.cpp
)

target_link_libraries(
    ${PROJECT_NAME} PUBLIC cpp-skeleton
)
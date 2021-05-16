cmake_minimum_required(VERSION 3.16)

# Set the project name
project(cpp-skeleton-test)

add_executable(
    ${PROJECT_NAME}
    main.cpp
    test.cpp
)

add_test(CppSkeletonTest cpp-skeleton-test)

target_link_libraries(
    ${PROJECT_NAME} PUBLIC gtest cpp-skeleton
)
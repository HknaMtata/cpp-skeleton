cmake_minimum_required(VERSION 3.16)

# Set the project name
project(cpp-skeleton-test)

add_executable(
    ${PROJECT_NAME}
    main.cpp
    test.cpp
)

add_test(NAME ${PROJECT_NAME} COMMAND ${PROJECT_NAME} WORKING_DIRECTORY ${CTEST_OUTPUT_DIRECTORY})

target_link_libraries(
    ${PROJECT_NAME} PUBLIC gtest cpp-skeleton
)
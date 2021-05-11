cmake_minimum_required(VERSION 3.20)

project(cpp-skeleton-project)

enable_testing()

set(GOOGLE_TEST_DIR submodules/googletest)
set(GOOGLE_TEST_INCLUDES ${GOOGLE_TEST_DIR}/googletest/include ${GOOGLE_TEST_DIR}/googlemock/include)

add_compile_options(
    -std=c++17
    -g
    -O2
    -pedantic
    -Wall
    -Wextra
    -Werror
    -Wshadow
    -Wsign-conversion
    -Wunreachable-code
    -fmax-errors=5
)

# Add sub directories
add_subdirectory(${GOOGLE_TEST_DIR})
add_subdirectory(src)
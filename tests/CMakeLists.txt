cmake_minimum_required(VERSION 3.0)

set(NAME c_matrix_tests)

add_executable(${NAME} main.c c_matrix/c_matrix_test.h)

target_include_directories(${NAME} PRIVATE "${PROJECT_SOURCE_DIR}/include")

target_link_libraries(${NAME} PRIVATE c_matrix)
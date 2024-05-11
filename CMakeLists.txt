cmake_minimum_required(VERSION 3.28)
project(lab14 C)

set(CMAKE_C_STANDARD 11)

add_executable(lab14 main.c
        libs/data_structures/vector/vector.c
        libs/data_structures/vector/vector.h
)

add_subdirectory(libs)
target_link_libraries(lab14 data_structures)


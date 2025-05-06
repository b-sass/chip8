cmake_minimum_required(VERSION 3.31)
set(CMAKE_C_STANDARD 17)
set(CMAKE_C_STANDARD_REQUIRED ON)

project(chip8 C)

file(GLOB_RECURSE SRC_FILES src/*.c)
add_executable(chip8 ${SRC_FILES})
target_include_directories(chip8 PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)
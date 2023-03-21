cmake_minimum_required(VERSION 3.1)

project(http-server
    VERSION 0.1.0
    LANGUAGES C
)

message(STATUS "CMake for ${PROJECT_NAME} v${PROJECT_VERSION}\n")

include_directories(${PROJECT_SOURCE_DIR}/src)

file(GLOB_RECURSE SOURCES src/*.c src/*.h)

add_executable(http-server ${SOURCES})
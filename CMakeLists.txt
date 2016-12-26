cmake_minimum_required(VERSION 3.7)

project(rirc)

file(GLOB_RECURSE RIRC_SOURCES src/*.c src/*.h)

find_package(Threads REQUIRED)

add_executable(rirc ${RIRC_SOURCES})
target_link_libraries(rirc Threads::Threads)


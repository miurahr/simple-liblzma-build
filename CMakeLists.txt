cmake_minimum_required(VERSION 3.16)
project(bcjdebug C)
set(CMAKE_CXX_STANDARD 11)
add_executable(test_bcj_file test_bcj_file.c)

add_subdirectory(liblzma)

target_link_libraries(test_bcj_file PRIVATE LibLZMA)
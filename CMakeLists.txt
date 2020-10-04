cmake_minimum_required(VERSION 3.16)
project(bcjdebug C)
set(CMAKE_CXX_STANDARD 11)

add_subdirectory(liblzma)
add_executable(test_bcj_file tests/test_bcj_file.c)
target_link_libraries(test_bcj_file PRIVATE LibLZMA)

cmake_minimum_required(VERSION 3.0)
project(cre2 C CXX)

add_library(cre2 STATIC
        src/cre2.cpp
        src/cre2.h
        )

target_include_directories(cre2 PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/../re2/)
target_compile_options(cre2 PRIVATE -fPIC)

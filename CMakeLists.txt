cmake_minimum_required(VERSION 3.14 FATAL_ERROR)

project(microhex LANGUAGES C)

add_library(microhex SHARED microhex.h microhex.c)
target_compile_features(microhex PRIVATE c_std_99)
target_include_directories(microhex PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

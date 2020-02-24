cmake_minimum_required(VERSION 3.5)

project(Chapter07 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 14)

enable_testing()

find_package(GTest REQUIRED)
find_package(benchmark REQUIRED)

include_directories(${GTEST_INCLUDE_DIRS})

add_executable(fast_sort1 fast_sort1.C)
add_executable(fast_sort2 fast_sort2.C)
add_executable(fast_sort3 fast_sort3.C)
add_executable(fast_sort4 fast_sort4.C)

add_executable(is_class1 is_class1.C)
add_executable(is_class2 is_class2.C)
add_executable(is_class3 is_class3.C)

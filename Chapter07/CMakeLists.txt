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

add_executable(is_valid3 is_valid3.C)
add_executable(is_valid4 is_valid4.C)

add_executable(multiply1 multiply1.C)
add_executable(multiply2 multiply2.C)
add_executable(multiply3 multiply3.C)
add_executable(multiply4 multiply4.C)
add_executable(multiply5 multiply5.C)

add_executable(overload1 overload1.C)
add_executable(overload1a overload1a.C)
add_executable(overload1b overload1b.C)
add_executable(overload2 overload2.C)
add_executable(overload3 overload3.C)
add_executable(overload4 overload4.C)
#add_executable(overload5 overload5.C)
add_executable(overload6 overload6.C)

add_executable(sfinae1 sfinae1.C)
add_executable(sfinae1a sfinae1a.C)
add_executable(sfinae2 sfinae2.C)
add_executable(sfinae3 sfinae3.C)
add_executable(sfinae4 sfinae4.C)

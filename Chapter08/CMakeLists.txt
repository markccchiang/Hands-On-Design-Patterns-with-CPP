cmake_minimum_required(VERSION 3.5)

project(Chapter08 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 14)

enable_testing()

find_package(GTest REQUIRED)
find_package(benchmark REQUIRED)

include_directories(${GTEST_INCLUDE_DIRS})

add_executable(function_call function_call.C)
target_link_libraries(function_call benchmark::benchmark)

add_executable(not_equal not_equal.C)
add_executable(not_equal_friend not_equal_friend.C)
add_executable(registry registry.C)
add_executable(visitor visitor.C)

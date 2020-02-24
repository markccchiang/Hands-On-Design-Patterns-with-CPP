cmake_minimum_required(VERSION 3.5)

project(Chapter06 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 14)

enable_testing()

find_package(GTest REQUIRED)
find_package(benchmark REQUIRED)

include_directories(${GTEST_INCLUDE_DIRS})

add_executable(smartptr smartptr.C smartptr_extra.C)
target_link_libraries(smartptr benchmark::benchmark)

cmake_minimum_required(VERSION 3.5)

project(Chapter05 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 14)

enable_testing()

find_package(GTest REQUIRED)

include_directories(${GTEST_INCLUDE_DIRS})

add_executable(memory1 memory1.C)
target_link_libraries(memory1 ${GTEST_BOTH_LIBRARIES})

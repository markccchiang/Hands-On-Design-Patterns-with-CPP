cmake_minimum_required(VERSION 3.5)

project(Chapter10 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 14)

enable_testing()

find_package(GTest REQUIRED)
find_package(benchmark REQUIRED)

include_directories(${GTEST_INCLUDE_DIRS})

add_executable(malloc1 malloc1.C)
target_link_libraries(malloc1 benchmark::benchmark)
add_executable(malloc2 malloc2.C)
target_link_libraries(malloc2 benchmark::benchmark)
add_executable(malloc3 malloc3.C)
target_link_libraries(malloc3 benchmark::benchmark)

add_executable(ch10-smartptr smartptr.C)
target_link_libraries(ch10-smartptr benchmark::benchmark)

add_executable(string1 string1.C)
target_link_libraries(string1 benchmark::benchmark)
add_executable(string2 string2.C)
target_link_libraries(string2 benchmark::benchmark)

add_executable(vector1 vector1.C)
target_link_libraries(vector1 benchmark::benchmark)
add_executable(vector2 vector2.C)
target_link_libraries(vector2 benchmark::benchmark)

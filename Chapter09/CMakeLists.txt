cmake_minimum_required(VERSION 3.5)

project(Chapter09 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 14)

enable_testing()

find_package(GTest REQUIRED)
find_package(benchmark REQUIRED)

include_directories(${GTEST_INCLUDE_DIRS})

add_executable(city city.C)
add_executable(cout_chaining cout_chaining.C)

add_executable(named_args named_args.C named_args_extra.C)
target_link_libraries(named_args benchmark::benchmark)

add_executable(named_args1 named_args1.C named_args1_extra.C)
target_link_libraries(named_args1 benchmark::benchmark)

#add_executable(poly_chain1 poly_chain1.C)
add_executable(poly_chain2 poly_chain2.C)
#add_executable(poly_chain2a poly_chain2a.C)
add_executable(poly_chain3 poly_chain3.C)

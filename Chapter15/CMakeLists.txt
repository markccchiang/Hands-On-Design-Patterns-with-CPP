cmake_minimum_required(VERSION 3.5)

project(Chapter15 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)

enable_testing()

find_package(GTest REQUIRED)
find_package(benchmark REQUIRED)

include_directories(${GTEST_INCLUDE_DIRS})

add_executable(singleton_eager singleton_eager.C)
target_link_libraries(singleton_eager benchmark::benchmark)

add_executable(singleton_lazy_leaky singleton_lazy_leaky.C)
target_link_libraries(singleton_lazy_leaky benchmark::benchmark)

add_executable(singleton_meyers singleton_meyers.C)
target_link_libraries(singleton_meyers benchmark::benchmark)

add_executable(singleton_meyers_pimpl singleton_meyers_pimpl.C)
target_link_libraries(singleton_meyers_pimpl benchmark::benchmark)

add_executable(singleton_meyers_pimpl1 singleton_meyers_pimpl1.C)
target_link_libraries(singleton_meyers_pimpl1 benchmark::benchmark)

add_executable(singleton_noaccess singleton_noaccess.C)
target_link_libraries(singleton_noaccess benchmark::benchmark)

add_executable(singleton_static singleton_static.C)
target_link_libraries(singleton_static benchmark::benchmark)

add_executable(singleton_static1 singleton_static1.C)
target_link_libraries(singleton_static1 benchmark::benchmark)

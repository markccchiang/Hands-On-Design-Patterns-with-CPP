cmake_minimum_required(VERSION 3.5)

project(Chapter15 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)

enable_testing()

find_package(GTest REQUIRED)
find_package(benchmark REQUIRED)

include_directories(${GTEST_INCLUDE_DIRS})

add_executable(01_scoped_ptr 01_scoped_ptr.C)
add_executable(02_scoped_ptr 02_scoped_ptr.C)
add_executable(02a_scoped_ptr_bug 02a_scoped_ptr_bug.C)
add_executable(02b_scoped_ptr 02b_scoped_ptr.C)
add_executable(02c_scoped_ptr 02c_scoped_ptr.C)
add_executable(02d_scoped_ptr 02d_scoped_ptr.C)
add_executable(02e_scoped_ptr 02e_scoped_ptr.C)
add_executable(02f_scoped_ptr 02f_scoped_ptr.C)
add_executable(02g_scoped_ptr 02g_scoped_ptr.C)

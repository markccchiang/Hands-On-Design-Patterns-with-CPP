cmake_minimum_required(VERSION 3.5)

project(Chapter18 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)

enable_testing()

find_package(GTest REQUIRED)
find_package(benchmark REQUIRED)

include_directories(${GTEST_INCLUDE_DIRS})

add_executable(01_visitor 01_visitor.C)
add_executable(01a_visitor 01a_visitor.C)
add_executable(01b_visitor 01b_visitor.C)
add_executable(02_visitor_args 02_visitor_args.C)
add_executable(02a_visitor_retval 02a_visitor_retval.C)
add_executable(03_container_visitor 03_container_visitor.C)
add_executable(03a_composite_visitor 03a_composite_visitor.C)
add_executable(03b_serialization_visitor 03b_serialization_visitor.C)
add_executable(03c_serialization_visitor 03c_serialization_visitor.C)
add_executable(04_visitor_template 04_visitor_template.C)
add_executable(04a_visitor_template 04a_visitor_template.C)
add_executable(04b_visitor_template 04b_visitor_template.C)
#add_executable(04c_visitor_template 04c_visitor_template.C)
add_executable(05_acyclic_visitor 05_acyclic_visitor.C)
add_executable(05a_acyclic_visitor 05a_acyclic_visitor.C)
add_executable(05b_acyclic_visitor 05b_acyclic_visitor.C)
add_executable(06_static_visitor 06_static_visitor.C)
add_executable(07_serialize_visitor 07_serialize_visitor.C)
add_executable(07a_serialize_visitor 07a_serialize_visitor.C)

cmake_minimum_required(VERSION 3.5)

project(Chapter13 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)

enable_testing()

find_package(GTest REQUIRED)
find_package(benchmark REQUIRED)

include_directories(${GTEST_INCLUDE_DIRS})

add_executable(ctor_dtor_dynamic_type ctor_dtor_dynamic_type.C)
add_executable(ctor_dtor_static_type ctor_dtor_static_type.C)
add_executable(ctor_dtor_virtual_type ctor_dtor_virtual_type.C)
add_executable(poly_copy poly_copy.C)
add_executable(poly_copy_unique poly_copy_unique.C)
add_executable(poly_copy_unique_crtp1 poly_copy_unique_crtp1.C)
add_executable(poly_copy_unique_crtp2 poly_copy_unique_crtp2.C)
add_executable(type_registry type_registry.C)
add_executable(type_registry_unique type_registry_unique.C)
add_executable(unit_factory unit_factory.C)

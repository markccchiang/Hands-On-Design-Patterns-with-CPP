cmake_minimum_required(VERSION 3.5)

project(Chapter12 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)

enable_testing()

find_package(GTest REQUIRED)
find_package(benchmark REQUIRED)

include_directories(${GTEST_INCLUDE_DIRS})

add_executable(equal_friend_factory_crtp equal_friend_factory_crtp.C)
add_executable(friend_factory friend_factory.C)
add_executable(friend_nontemplate friend_nontemplate.C)
add_executable(friend_template friend_template.C)
add_executable(plus_friend plus_friend.C)
add_executable(plus_friend1 plus_friend1.C)
add_executable(plus_friend1_template plus_friend1_template.C)
add_executable(plus_friend_factory plus_friend_factory.C)
add_executable(plus_friend_factory_crtp plus_friend_factory_crtp.C)
add_executable(plus_friend_factory_ns plus_friend_factory_ns.C)
add_executable(plus_friend_template plus_friend_template.C)
add_executable(plus_member plus_member.C)

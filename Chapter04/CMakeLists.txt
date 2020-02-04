cmake_minimum_required(VERSION 3.5)

project(Chapter04 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 14)

add_executable(list_swap list_swap.C)
add_executable(member_swap member_swap.C)
add_executable(nonmember_swap_friend_forward nonmember_swap_friend_forward.C)
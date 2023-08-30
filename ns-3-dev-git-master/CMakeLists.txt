cmake_minimum_required(VERSION 3.10)

project(
  hello_world 
  VERSION 1.0
  LANGUAGES CXX)

add_library(mylib mptcp-subflow.h)
add_executable(main mptcp-example.cc)
target_link_libraries(main PRIVATE mylib)

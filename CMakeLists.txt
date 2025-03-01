cmake_minimum_required(VERSION 3.9)
project(libpid LANGUAGES C)

add_library(libpid PID.c PID.h)

add_executable(pid_test PID_Test.c)
target_link_libraries(pid_test libpid)
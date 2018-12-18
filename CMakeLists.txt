cmake_minimum_required(VERSION 2.6)
project(cacti)
aux_source_directory(. SRCS)
add_executable(cacti ${SRCS})

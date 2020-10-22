cmake_minimum_required(VERSION 3.17)
project(pcap_sniff C)

set(CMAKE_C_STANDARD 99)

add_library(pcap_sniff library.c library.h sniff.c)

set(GCC_COVERAGE_COMPILE_FLAGS "-lpcap")
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} ${GCC_COVERAGE_COMPILE_FLAGS}" )
cmake_minimum_required(VERSION 3.17)
project(pcap_sniff C)

set(CMAKE_C_STANDARD 99)

add_library(pcap_sniff library.c library.h)
cmake_minimum_required(VERSION 3.7)
project(style-sensitive-word-vectors)

set(CMAKE_CXX_STANDARD 14)

set(SOURCE_FILES pthread_barrier.h pthread_barrier.c distance_stylevec.c word2stylevec.c)
add_executable(Word2stylevec word2stylevec.c pthread_barrier.c)
add_executable(Distance distance_stylevec.c)

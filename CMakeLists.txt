cmake_minimum_required(VERSION 3.1)
project(lab4)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -D_FILE_OFFSET_BITS == 64 -m64 -std=c88")

set(SOURCE_FILES more.c term_out.c)
add_executable(lab4 ${SOURCE_FILES} term_in.h term_in.c commands.h commands.c positions.h positions.c lines.h lines.c)
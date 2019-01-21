project(fbv)
cmake_minimum_required(VERSION 2.8)
aux_source_directory(. DIR_SRCS)
add_executable(fbv ${DIR_SRCS})

target_link_Libraries(fbv png)
target_link_Libraries(fbv jpeg)

install(TARGETS fbv DESTINATION bin)

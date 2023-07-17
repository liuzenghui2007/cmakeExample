# 使用 aux_source_directory 命令可以查找某个路径下的所有源文件
cmake_minimum_required(VERSION 3.0)
project(CALC)
file(GLOB MAIN_SRC ${CMAKE_CURRENT_SOURCE_DIR}/src/*.c)
# file(GLOB MAIN_HEAD ${CMAKE_CURRENT_SOURCE_DIR}/include/*.h)


add_executable(app  ${MAIN_SRC})


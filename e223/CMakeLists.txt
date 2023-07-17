cmake_minimum_required(VERSION 3.0)
set(HOME ./)
set(EXECUTABLE_OUTPUT_PATH ${HOME}/bin)

project(CALC)
add_executable(app add.c div.c main.c mult.c sub.c)


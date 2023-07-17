# 使用set拼接
cmake_minimum_required(VERSION 3.0)
project(TEST)
set(TEMP "hello,world")
# 包含源文件
file(GLOB SRC_1 ${PROJECT_SOURCE_DIR}/src1/*.cpp)
file(GLOB SRC_2 ${PROJECT_SOURCE_DIR}/src2/*.cpp)
# 包含头文件路径
include_directories(${PROJECT_SOURCE_DIR}/include)
# 追加(拼接)
list(APPEND SRC_1 ${SRC_1} ${SRC_2} ${TEMP})
# 最后啥也不干，输出信息看看
message(STATUS "message: ${SRC_1}")

# 使用 set 命令可以创建一个 list
set(tmp1 a;b;c;d;e)
set(tmp2 a b c d e)
message(${tmp1})
message(${tmp2})

CMAKE_MINIMUM_REQUIRED(VERSION 3.12)

PROJECT(nonius)

#[[
也就是这个两个函数的作用应该差不多
一个区别是：
target_link_libraries 要在 add_executable 之后
link_libraries 要在 add_executable 之前
]]

link_libraries(pthread)
include_directories(${PROJECT_SOURCE_DIR}/include/)


add_executable(examples1 examples/example1.c++)
add_executable(examples2 examples/example2.c++)
add_executable(examples3 examples/example3.c++)
add_executable(examples4 examples/example4.c++)
add_executable(examples5 examples/example5.c++)
add_executable(examples6 examples/example6.c++)
add_executable(examples7 examples/example7.c++)




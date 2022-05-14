# CMakeList.txt: 顶层 CMake 项目文件，在此处执行全局配置
# 并包含子项目。
#
cmake_minimum_required (VERSION 3.12)

project ("CMakeProject1")

# 设置为C++11标准
SET(CMake_CXX_STANDARD 11)

include_directories(my_json_parser)

# 包含子项目。
add_subdirectory ("my_json_parser")
add_subdirectory ("lib/googletest")
add_subdirectory ("test")
#

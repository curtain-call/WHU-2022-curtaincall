# CMakeList.txt: CMakeProject1 的 CMake 项目，在此处包括源代码并定义
# 项目特定的逻辑。
#
cmake_minimum_required (VERSION 3.12)

# 将源代码添加到此项目的可执行文件。(如果是编译库文件的话，好像不需要.exe,报链接器错误，等csapp第七章讲完看)
#add_executable (praser_run "src/praser_lite.cpp" "header/praser_lite.h" "header/file_operation.h")

add_library (parser_lib STATIC "src/praser_lite.cpp" "header/praser_lite.h" "header/file_operation.h")

# TODO: 如有需要，请添加测试并安装目标。
set(CMAKE_CXX_STANDARD 11)

#target_link_libraries(${PROJECT_NAME} jsoncpp_lib) 
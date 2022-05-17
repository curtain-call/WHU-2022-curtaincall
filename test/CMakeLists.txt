#set(BINARY ${CMAKE_PROJECT_NAME}_tst)
#file(GLOB_RECURSE TEST_SOURCES LIST_DIRECTORIES true *.h *.cpp)
#set(SOURCES ${TEST_SOURCES})
add_executable(parser_tst "main.cpp" "parser_test.cpp")
add_test(NAME parser_tst COMMAND parser_tst)
# 链接src生成的lib库和gtest库,自然完成测试
target_link_libraries(parser_tst PUBLIC parser_lib gtest) 
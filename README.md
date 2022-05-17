## github版本控制经验记录
- 更改缓存：
- 更改仓库缓存边带
  全局的：git config –global sendpack.sideband false
  仓库的：git config –local sendpack.sideband false
- 先git pull再push

## CMake

引入外部库时不能使用fetchcontent，因为vs2017的支持直到v3.12
## subdirectory

### my_json_parser
- 采用googletest搭建测试框架
- 采用TDD(test-drive development) 开发模式
- 2022.5.14 
  initialized；
  completed the "null" "true" "false" part;
  
## change log
- 2022.5.14 添加my_json_parser子项目

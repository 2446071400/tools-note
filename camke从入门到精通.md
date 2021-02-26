[学习网址](https://blog.csdn.net/afei__/article/details/81201039)
# Cmakelists.txt
## 基础
1. 不区分大小写
## 语法
1. cmake_minimum_required(VERSION 3.10) 指定cmake要求的最低版本 //
这行命令是可选的，我们可以不写这句话，但在有些情况下，如果 CMakeLists.txt 文件中使用了一些高版本 cmake 特有的一些命令的时候，就需要加上这样一行，提醒用户升级到该版本之后再执行 cmake。
2. project(demo) 设置项目名称 ///这个命令不是强制性的，但最好都加上。它会引入两个变量 demo_BINARY_DIR 和 demo_SOURCE_DIR，同时，cmake 自动定义了两个等价的变量 PROJECT_BINARY_DIR 和 PROJECT_SOURCE_DIR。
3. add_executable(demo demo.cpp) 设置编译类型为生成可执行文件
4. add_library(common STATIC util.cpp) 设置编译类型为生成静态库
5. add_library(common SHARED util.cpp) 设置编译类型为生成动态库


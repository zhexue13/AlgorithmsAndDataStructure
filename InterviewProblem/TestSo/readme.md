### 测试生成动态链接库
#### 重点笔记
- 使用-fPIC　-shared 编译选项生成动态链接库，第一个选项是以地址无关的模式生成。
- makefile文件的编写注意$@ $^的用法。前者是目标集合，后者是依赖集合，就是不用写文件名。
- 使用时可以用-L. -lname来指定链接动态库。
#### 执行方法
1. make生成a.out和.so文件，./a.out执行测试程序。
#### 补充说明如何查看动态库的符号
可以使用nm -D 或者objdump -tT 查看动态库符号。

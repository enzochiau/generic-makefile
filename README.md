# GenericMakefile

A generic makefile for use with small/medium C and C++ projects.

# Introduction

- GenericMakefile目录包含C程序和C++程序的各自Makefile. 
- gcmakefile-0.5目录包含一处通用的C/C++程序Makefile，以及一个gtk实例. (`推荐使用`)

# 一般使用方法

- 将Makefile拷贝到源代码目录
- 修改生成的目标代码名称(a.out, target-name, *.so)
- 添加编译参数，可能要指定.h文件目录 `-I`
- 添加链接选项，如`-lpthread`
- 如果要生成so，请参考[here](http://onestraw.net/linux/linux-ld/)来添加编译和链接选项

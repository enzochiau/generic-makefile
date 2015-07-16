gnu make
-----------

x ?= value

如果x没有值，那么执行正常幅值


make -C $subdir

make子目录subdir下的makefile

#内置变量

`CURDIR`: 代表make当前工作目录  
`$@` 	表示规则中的目标。  
`$<` 	表示规则中的第一个条件。  
`$?` 	表示规则中所有比目标新的条件，组成一个列表，以空格分隔。  
`$^` 	表示规则中的所有条件，组成一个列表，以空格分隔。  

    main: main.o stack.o maze.o
        gcc main.o stack.o maze.o -o main
    
$@ 表示 main  
$< 表示 main.o  
$^ 表示 main.o stack.o maze.o   

- http://hahack.com/wiki/tools-makefile.html

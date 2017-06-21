# hello_C


gcc -E hello.c -o hello.i
E 参数 通知gcc对目标文件进行预编译，这里是对文件hello.c文件
o 参数 是对命令输出结果进行导入操作，这里是把 gcc -E hello.c 操作结果输出到文件hello.i（命名要自定义）中进行保存

gcc -S hello.i -o hello.s
S 参数 通知gcc对目标文件进行编译，这里是对文件hello.i文件

gcc -c hello.s -o hello.o
c 参数 通知gcc对目标文件执行指令转换操作

gcc hello.o -o hello
这里我们就得到了一个可以直接在系统下执行的文件 hello

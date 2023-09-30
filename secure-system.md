# 安全系统
修改部分内核和文件系统代码，更好地控制各个程序的syscall

新建两个syscall，实现如下函数

```c
asmlinkage long lock(
  int syscall_id; //ID of the target syscall
  char * filename; //executable file name
  int pwd; //set pwd
); //make <filename> can use <syscall_id>

asmlinkage long unlock(
  int syscall_id; //ID of the target syscall
  char * filename; //executable file name
  int pwd; //set pwd
); //make <filename> can't use <syscall_id>
```
其中pwd是动态的；

同时提高部分文件权限


# 联合语言
把许多语言合并到一起，一个文件可以有多个语言
如：
```
#include<stdio.h> // c
import random # python
int main(){
  int r = random.randint(0,100); // union
  if r >= 50: # python
    console.log(r); // js
  else:
    printf("%d",r);
  return r 
}
```
打算用图分析语法
```
line 1-\           /6\
         >-3{-4-5<     >9}
line 2-/           \8/
```
并支持通过IR转换为任意语言，同时做到快、安全

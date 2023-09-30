# 联合语言
把许多语言合并到一起，即一个文件可以有多个语言
如：
```
#include<stdio.h> // c
import random # python
int main(){
  int r = random.randint(0,100); // union
  if r >= 50: # python
    console.log(r);
  else:
    printf("%d",r);
  return r 
}

# C范例代码训练
## 第一章 c语言程序基本结构
### 1. 函数的基本结构
#### 1.1 第一个c语言程序
##### 1.1.1 用c语言实现"helloworld!"字符串的打印
```
#include <stdio.h>

int main(void)
{
    printf("hello world !!"\n);
    return 0;
}
```
##### 1.1.2 函数返回值-return 语句
```
#include <stdio.h>

int foo(void)
{
    return 5;
}

int main(void)
{
    int a = foo();
    return a;
}
```
##### 1.1.3 全局变量及同名局部变量
```
#include <stdio.h>

int b;
int c;
int d;

int main(int argc,char *argv[])
{
    int a;
    int c = 5; 
    int d = 6;
    return 0;
}
```

#### 1.2 自定义函数
##### 1.2.1 函数的定义，声明
```
#include <stdio.h>

int goo(int d, int e, int f)
{
    int g = d + e;
    return f;
}

int swap(int a, int b);

int foo()
{
    return 0；
}

int main(void)
{
    int x,y;
    x = -1 ; y = 2;
    printf("%d,%d\n",x,y);
    swap(x,y);
    printf("%d,%d\n",x,y);
    printf("%d\n",goo(2,3,4));

    foo(1,2,34,5)

    return 0;
}

int swap(int a, int b)
{
    int tmp =  a; 
    a = b ; 
    b = tmp ; 
    return 0;
}
```
##### 1.2.2 自定义函数应用
```
#include <stdio.h>

int add(int a, int b)
{
    return a+b;
}

int sub(int a, int b)
{
    return a-b;
}

int main(void)
{
    int ret;
    printf("hello, Cruel World!\n");
    ret = add(100,200);
    printf("add = %d \n",ret);
    ret = sub(100,200);
    printf("sub = %d \n",ret);

    return 0;
}
```
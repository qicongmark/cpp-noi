## C++基础题库（四）

```
包含 C++ 编程的基础知识，适用于C++编写学习或信奥赛C++考试练习。

选择题 20 道，答对 15 道即算通过。
```

### 一、选择题（共 20 题）

#### 1、以下正确的函数定义是（ ）

A. int fun4(int a, int b) { return a+b; }

B. void fun4(int a, int b) { return a+b; }

C. int fun4(int a, int b) { fun4 = a+b; }

D. void fun4(int a, int b){ fun4 = a+b; }

#### 2、以下正确的函数定义是（ ）

A. void fun5();{ cout<<"Call f5\n"; }

B. void fun5() { return f5; }

C. void fun5() { cout<<"Call f5\n"; }

D. void fun5() { return 5; }

#### 3、有函数原型 void fun6( int ); 在下列选项中，不正确的调用是（ ）

A. int a = 21; fun6( a );

B. int a = 15; fun6( a*3 );

C. int b = 100; fun6( &b );

D. fun6( 256 );

#### 4、有函数原型 void fun7( int * ); 在下列选项中，正确的调用是（ ）

A. double x = 2.17; fun7( &x );

B. int a = 15; fun7( a*3.14 );

C. int b = 100; fun7( &b );

D. fun7( 256 );

#### 有函数原型 void fun8( int & ); 在下列选项中，正确的调用是（ ）

A. int a = 2.17; fun8( &a );

B. int a = 15; fun8( a*3.14 );

C. int b = 100; fun8( b );

D. fun8( 256 );

#### 6、有以下声明，在下列选项中，正确的调用是（ ）

```
void fun9( int * & ); 
int a;
int *p = &a;
```

A. fun9(&a);

B. fun9(p);

C. fun9(*a);

D. fun9(*p);

#### 7、以下正确的函数定义是（ ）

A. int * fun10(double x){ return x; }

B. int * fun10(double x){ return &x; }

C. int * fun10(int a){ return *a; }

D. int * fun10(int a){ return &a; }

#### 8、函数参数的默认值不允许为（ ）

A. 全局常量

B. 直接常量

C. 局部变量

D. 函数调用

#### 9、一个项目中只能有一个的函数是（ ）

A. 系统库函数

B. 自定义函数

C. 主函数

D. 在其他文件中定义的函数

#### 10、实现函数调用需要（ ）进行信息管理

A. 队列

B. 堆栈

C. 数组

D. 参数

#### 11、一个项目中包含三个函数：main、fa 和 fb 函数，它们之间不正确的调用是（ ）

A. 在 main 函数中调用 fb 函数

B. 在 fa 函数中调用 fb 函数

C. 在 fa 函数中调用 fa 函数

D. 在 fb 函数中调用 main 函数

#### 12、关于递归调用不正确的描述是（ ）

A. 递归调用和嵌套调用都是通过堆栈管理实现的

B. 函数直接或间接调用自己称为递归调用

C. 递归终止条件必须为参数值等于 0

D. 递归算法的问题规模必须是逐步缩

#### 13、有数组定义 double d[10]; 以下叙述不正确的是（ ）

A. 数组 d 有 10 个元素

B. 数组 d 的最后一个元素是 d[10]

C. 数组 d 的第一个元素 *d

D. 数组 d 的字节数是 sizeof(double)*10

#### 14、以下对一维数组 a 的定义正确的是（ ）

A. int n = 5, a[n];

B. int a(5);

C. const int N = 5; int a[N];

D. int n; cin>>n; int a[n];

#### 15、下列数组定义语句中，不合法的是（ ）

A. int a[3] = { 0, 1, 2, 3 };

B. int a[] = { 0, 1, 2 };

C. int a[3] = { 0, 1, 2 };

D. int a[3] = { 0 };

#### 16、已知 int a[10] = { 0, 1, 2, 3, 4, 5, 6, 7, 8, 9 }, *p = a; 以下不能表示数组 a 中元素的表达式是（ ）

A. *a

B. *p

C. a

D. a[p-a]

#### 17、已知 int a[] = { 0,2,4,6,8,10 }, *p = a+1; 其值等于 0 的表达式是（ ）

A. *(p++)

B. *(++p)

C. *(p--)

D. *(--p)

#### 18、声明一个长度为 10 的数组，元素类型为整型指针的正确语句是（ ）

A. int *pary[10];

B. int (*pary)[10]；

C. int *pary(10);

D. int **pary[10];

#### 19、有以下语句，则能够输出 a+b+c 的值的语句是（ ）

```
int a=1, b=2, c=3; 
int *pary[3]={&a, &b, &c};
```

A. cout<<(pary[0]+pary[1]+pary[2]);

B. cout<<(*pary[0]+*pary[1]+*pary[2]);

C. cout<<(pary[1]+pary[2]+pary[3]);

D. cout<<(*pary[1]+*pary[2]+*pary[3]);

#### 20、以下不能对二维数组 a 进行正确初始化的语句是（ ）

A. int a[2][3] = { 0 };

B. int a[][3] = { { 0,1 }, { 0 } };

C. int a[2][3] = { { 0, 1 }, { 2, 3 }, { 4, 5 } };

D. int a[][3] = { 0, 1, 2, 3, 4, 5 };



---



### 参考答案

1~5：ACCCC

6~10：BDCCB

11~15：DCBCA

16~20：CDABC




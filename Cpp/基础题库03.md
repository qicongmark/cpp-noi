```
包含 C++ 编程的基础知识，适用于C++编写学习或信奥赛C++考试练习。

选择题 20 道，答对 15 道即算通过。
```

### 一、选择题（共 20 题）

#### 1、已知 int i=0, x=1, y=0; 在下列选项中，使 i 的值变成 1 的语句是（ ）

A. if( x&&y ) i++;

B. if( x==y ) i++;

C. if( x||y ) i++;

D. if( !x ) i++;

#### 2、已知 int i=0, x=1, y=0; 在下列选项中，使 i 的值变成 1 的语句是( )

A. if( x ) { if(y) i=1; else i=0; }

B. if( x ) {if(y) i=1; } else i=0;

C. if( x ) i=0; else { if(y) i=1; }

D. if( x ) i=1; else {if(y) i=0; }

#### 3、设 i=2，执行下列语句后 i 的值为（ ）

```
switch( i )
{ 
    case 1 : i ++;
    case 2 : i --;
    case 3 : ++ i; break;
    case 4 : -- i;
    default : i ++;
}
```

A. 1

B. 2

C. 3

D. 4

#### 4、执行下列语句后，输出显示为（ ）

```
char ch='A';
switch( ch )
{ 
    case 'A' : ch++;
    case 'B' : ch++;
    case 'C' : ch++;
}
cout<<ch<<endl;
```

A. A

B. B

C. C

D. D

#### 5、已知 int i=0，x=0; 在下面 while 语句执行时循环次数为（ ）

```
while( !x && i< 3 ) 
{ 
    x++; 
    i++; 
}
```

A. 4

B. 3

C. 2

D. 1

#### 6、已知 int i=3; 在下面 do-while 语句执行时的循环次数为（ ）

```
do {
    i--; 
    cout<<i<<endl; 
}while( i!= 1);
```

A. 1

B. 2

C. 3

D. 4

#### 7、以下程序段形成死循环的是（ ）

A. int x; for( x=0; x<3; ) { x++; };

B. int k = 0; do { ++k; } while( k>=0 );

C. int a=5; while( a ) { a--; };

D. int i=3; for(; i; i -- );

#### 8、有“if<逻辑表达式><语句>;”，当整型变量 a 和 b 的值都不等于 0 时执行<语句>，则逻辑表达式是（ ）

A. a & b

B. a && b

C. a != b

D. a - b != 0

#### 9、有“if<逻辑表达式><语句>;”，当整型变量 a、b 的值相等时执行<语句>，则逻辑表达式是（ ）

A. a=b

B. a!=b

C. a-b

D. !(a-b)

#### 10、有以下语句，输出结果是（ ）

```
for( int i=1; i<=10; i++)
{
 if(!(i%3)) cout << i << " ";
}
```

A. 1 2 3

B. 1 2 4 5

C. 3 6 9

D. 4 5 6

#### 11、有以下语句，执行完成后 sum 的值是（ ）

```
int i=5, sum=0;
while(i--) { sum+=i%2; }
```

A. 2

B. 3

C. 4

D. 5

#### 12、有如下语句，循环体执行的次数是（ ）

```
int a=5, b=1;
while(a-b) { 
    a--; 
    b++; 
}
```

A. 1

B. 2

C. 3

D. 4

#### 13、下面 for 语句执行时的循环次数为（ ）

```
int i, j;
for ( i=0, j=5; i=j; )
{ 
    cout<<i<<j<< endl; 
    i++; 
    j--; 
}
```

A. 0

B. 5

C. 10

D. 无限

#### 14、执行以下程序段后，x 的值是（ ）

```
int i, j, x = 0;
for( i=0; i<=3; i++ )
{ 
    x++;
    for( j=0; j<=3; j++ )
    { 
        if( j ) continue;
        x++;
    } 
}
```

A. 8

B. 12

C. 14

D. 16

#### 15、考察 break 用法，以下程序段输出结果是（ ）

```
int i,n=0;
for(i=0; i<10; i++)
{ 
    if( i%3 ) break;
    n++;
}
cout<<n<<endl;
```

A. 1

B. 2

C. 3

D. 4

#### 16、考察continue用法，以下程序段输出结果是（ ）

```
int i,n=0;
for(i=0; i<10; i++)
{ 
    if( i%3 ) continue;
    n++;
}
cout<<n<<endl;
```

A. 1

B. 2

C. 3

D. 4

#### 17、考察 goto 的用法，以下程序段输出结果是（ ）

```
int i,n=0;
for(i=0; i<10; i++)
{ 
    if( i>2 ) goto out;
    n++;
}
out: cout<<n<<endl;
```

A. 1

B. 2

C. 3

D. 4

#### 18、以下正确的函数原型为（ ）

A. fun1( int x; int y );

B. void fun1( x, y );

C. void fun1( int x, y );

D. void fun1( int, int );

#### 19、有函数原型 int f2(int, int); 以下正确的调用语句是（ ）

A. int a=fun2(1);

B. cout<<fun2(3,4);

C. int a=fun2(1)+fun(2);

D. cout<<fun2(3+4);

#### 20、有函数原型 void f3(double); 以下正确的调用语句是（ ）

A. double a=fun3(0.15);

B. fun3(0.34);

C. double a=fun3(0.1)+f3(0.2);

D. cout<<fun3(3.4);



---



### 参考答案

1~5：CDBDD

6~10：BBBDC

11~15：ABBAA

16~20：DCDBB




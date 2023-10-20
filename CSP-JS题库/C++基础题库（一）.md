## C++基础题库（一）

```
包含 C++ 编程的基础知识，适用于C++编写学习或信奥赛C++考试练习。

选择题 20 道，答对 15 道即算通过。
```

### 一、选择题（共 20 题）

#### 1、一个可运行的C＋＋源程序 （ ）

A. 由一个或多个主函数构成

B. 仅由一个主函数和零个以上（含零个）的子函数构成

C. 仅由一个主函数构成

D. 由一个且只有一个主函数和多个子函数构成

#### 2、使用标准命名空间的语句是（ ）

A. using namespace std;

B. using namespace iostream;

C. include std;

D. include iostream;

#### 3、控制台程序中需要使用 cin 和 cout 输出/输入，因此 include 指令包含的头文件是（ ）

A. cmanth

B. conio.h

C. iostream

D. iomanip

#### 4、C＋＋程序的三种基本结构是（ ）

A. 顺序结构、选择结构、循环结构

B. 递归结构、循环结构、转移结构

C. 嵌套结构、递归结构、顺序结构

D. 循环结构、转移结构、顺序结构

#### 5、有语句 double x, y; 以下正确的输入语句是（ ）

A. cin<<x, y;

B. cin<<x+y;

C. cin<<x<<y<<endl;

D. cin>>x>>y;

#### 6、下列哪个不是C++的基本数据类型（ ）

A. string

B. int

C. float

D. double

#### 7、在C++中，以下哪个是输入流对象？（ ）

A. cout

B. cin

C. endl

D. cerr

#### 8、下列代码输出的结果是什么（ ）

```
#include <iostream>
using namespace std;

int main() {
    int x = 5;
    int y = 2;
    cout << x / y << "  ";
    cout << x % y ;
    return 0;
}
```

A. 2 1

B. 2 0

C. 2.5 0.5

D. 2.5 1.5

#### 9、在C++中，以下哪个关键字可以用来定义一个变量，使得它的值在程序执行期间不可更改（ ）

A. const

B. static

C. volatile

D. mutable

#### 10、主函数 main 的定义包含四部分（ ）

```
int main()
{
    return 0;
}
```

A. 返回值类型 int 和 返回值 return 0;

B. 函数名 main 和 函数体 {}

C. 参数列表 ()

D. 以上说法都正确

#### 11、对 C++语言和 C语言的兼容性，描述正确的是（ ）

A. C++ 兼容 C

B. C 兼容 C++

C. C++ 不兼容 C

D. 二者没有任何兼容关系

#### 12、在 C++中使用流进行输入输出，其中用于屏幕输出的对象是（ ）

A. cerr

B. cin

C. cout

D. cfile

#### 13、C++ 中注释 “//”的有效范围是（ ）

A. 从“//”开始到行尾

B. 从“//”开始到下一个 “//”

C. 从“//”开始到程序尾

D. 以上说法都不对

#### 14、表达式 4%(-3) 和 -4%3 的值为（ ）

A. -1 和 -1

B. 1 和 -1

C. -1 和 1

D. 1 和 1

#### 15、下列选项不是 C++关键字的是（ ）

A. int

B. void

C. class

D. i

#### 16、结构化程序设计所规定的三种基本控制结构是（ ）

A. 输入、处理、输出

B. 树形、网形、环形

C. 顺序、选择、循环

D. 主程序、子程序、函数

#### 17、下列变量的初始化和赋值语句，哪个是错的（ ）

A. int age = 100；

B. int age;age = 100;

C. int age=100, name;

D. int age; name;

#### 18、下列关于单目运算符++、--的叙述中正确的是（ ）

A. 它们的运算对象可以是任何变量和常量

B. 它们的运算对象可以是char型变量和int型变量，但不能是float型变量

C. 它们的运算对象可以是int型变量，但不能是double型变量

D. 它们的运算对象可以是char型变量、int型变量和float型变量

#### 19、设有以下程序，哪个语句是错误的（ ）

```
#include <iostream>
#define d 2
using namespace std;

int main()
{
    int a=0;
    double b=1.25;
    char c='A';
    a++;
    b++;
    c++;
    d++;
}
```

A. a++

B. b++

C. c++

D. d++

#### 20、以下选项中，与 k=n++ 完全等价的表达式是（ ）

A. k=n; n=n+1;

B. n=n+1; k=n;

C. k=++n;

D. k+=n+1;





---



### 参考答案

1~5：BACAD

6~10：ABAAD

11~15：ACABD

16~20：CDDDA




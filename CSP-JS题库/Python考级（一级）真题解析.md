### 青少年编程（Python）等级考试（一级试卷）

> 蓝桥杯、白名单考级
>
> 爱码岛编程课堂 — 帮助千万家庭学好编程
>
> 信息学奥赛 · 蓝桥杯 · 升学 · 逻辑思维 · 编程和数学
>
> 讲师：祁聪 





### 一、选择题（共 25 题，共50分）



#### 1、表达式 len("学史明理增信，读史终生受益") > len("reading history will benefit you")的结果是（ ）

A. 0

B. True

C. False

D. 1



**参考答案：C**

在Python中，表示“假的”、“错误”，使用`False`关键字；表示“真的”、“对的”，使用`True`关键字。

`len()`是length的缩写，表示计算字符内容的长度，数一数就知道前面的长度是13，后面的长度是32。

那么 `13 > 32` 吗？很显然是错误的，也就是 `False`，所以选择 C。

```python
#编程练习
a = len("学史明理增信，读史终生受益")
b = len("reading history will benefit you")

print(a)
print(b)
print(a > b)
print(len("学史明理增信，读史终生受益") > len("reading history will benefit you"))
```



#### 2、表达式(2<1)==False 的结果是？（ ）

A. None

B. True

C. Error

D. False



**参考答案：B**

`2 < 1`是错的，所以这个运算得到的结果是 `False`，然后 `==`是比较是否相等的意思，也就是说 `False`和`False`是相等的吗？ 很显然是，所以结果是 `True`

```python
#编程练习
print((2<1) == False)
```



#### 3、在 Python shell 中运行 type('6' * 20)，运行结果为？（ ）

A. <class 'int'>

B. <class 'str'>

C. <class 'float'>

D. 语法错误



**参考答案：B**

`type()`函数表示得到数据类型，比如`type(3)`表示整数。

`'6' * 20` 虽然有 20 数字，但是前面的6加了单引号，在Python中，单引号或双引号包含的内容，都表示字符串类型。这个表达式表示的是`'6'`这个字符重复20次。

```python
#编程练习
print(type(3))

print('6' * 20)
print(type('6' * 20))
```



#### 4、关于 turtle 的运动体系中，说法正确的是？（ ）

A. turtle.goto(x,y)可以让小海龟直线前进到指定的坐标位置。 

B. turtle.forward(a)可以让小海龟向前移动 a 个像素，如果 a 为负数，运动方向不变，只是小海龟 

自身的方向与原来相反。 

C. turtle.seth()、turtle.left()、turtle.right()的参数均为绝对角度。 

D. turtle.dot()与 turtle.circle()的参数均为半径。



**参考答案：A**

主要目的是考察`turtle`的函数用法。

B：错误原因是，运动方向是反方向，自身方向不变。

C：`seth`使用的是绝对角度。

D：dot是一个点，参数为直径。

官方文档：https://docs.python.org/zh-cn/3/library/turtle.html

```python
#编程练习
import turtle

pen = turtle.Turtle()
pen.pensize(3)

# pen.dot(100)
# pen.circle(100)

# pen.goto(500,300) #goto到坐标(500,300)
# pen.forward(-500)

pen.forward(500)
# pen.seth(270)
# pen.right(90)
# pen.forward(500)
```



#### 5、在 turtle 画图中，常常使用 turtle.color(color1, color2)指令进行画笔颜色和填充颜色的设置， 下列关于该指令使用正确的是？（ ） 

A. turtle.color(“red”, ”yellow”)表示画笔颜色为黄色，背景颜色为红色。 

B. turtle.color(“red”)表示画笔颜色为红色，背景颜色随机。 

C. turtle.color(color1,color2)指令中的参数 color2 是可选项，可以只有一个颜色参数。 

D. turtle.color(color1,color2)指令中若将 color1 和 color2 删掉，即turtle.color()，小海龟在向前走 100 像素时，画布不会出现小海龟的轨迹。



**参考答案：C** 

A：第二个参数，是填充颜色，要配合`begin_fill()`和`end_fill()`使用

B：背景色默认白色，不是随机

D：画笔默认是黑色，填充颜色也是默认黑色

```python
#编程练习
import turtle

pen = turtle.Turtle()

pen.pensize(3)
pen.color('red','yellow')

pen.begin_fill()
pen.circle(100)
pen.end_fill()
```





#### 6、如图所示，想要将一行输出的两句诗词，变成二行输出方式，应该如何写输出指令？（ ） 

![image-20230828161947576](./imgs/image-20230828161947576.png)



A. print("床前明月光，疑是地上霜") 

B. print("""床前明月光 疑是地上霜""") 

C. print("床前明月光 

疑是地上霜") 

D. print("""床前明月光 

疑是地上霜""") 



**参考答案：D** 

在Python中实现换行使用的是`"""`包含起来

```python
#编程练习
print("""床前明月光 
疑是地上霜""") 
```



#### 7、绘制一个半径为 5 的红色圆点，下列选项不正确的是？（ ） 

A. 

import turtle 

turtle.color("red") 

turtle.dot(10) 

turtle.done() 

B. 

import turtle 

turtle.color("red","red") 

turtle.begin_fill()

turtle.circle(5) 

turtle.end_fill() 

turtle.done() 

C. 

import turtle 

turtle.pencolor("red") 

turtle.dot(10) 

turtle.done() 

D. 

import turtle 

turtle.color("red") 

turtle.dot(5) 

turtle.done() 

 

**参考答案：D** 

dot的参数是直径，而不是半径。





#### 8、下列指令可以方便将画笔设置回到初始位置和初始方向的是？（ ） 

A. turtle.home() 

B. turtle.clear() 

C. turtle.goto() 

D. turtle.setup() 



**参考答案：A**

B：用画笔清空画的内容

C：直线前进到指定的坐标位置

D：turtle设置绘画窗口大小、位置



```python
#编程练习
import turtle

turtle.setup(500,600,10,10)

pen = turtle.Turtle()
pen.pensize(3)

pen.goto(500,0)

pen.home()
pen.clear()
```



#### 9、如图所示，turtle.circle(100)是绘制一个半径为 100 的圆，请问画笔从以下哪个点出发开始绘制？ （ ） 

<img src="./imgs/image-20230828162959276.png" alt="image-20230828162959276" style="zoom:50%;float:left;" />

A. A 

B. B 

C. C 

D. D 



**参考答案：A**

```python
#编程练习
import turtle

pen = turtle.Turtle()
pen.pensize(3)
pen.circle(100)
```



#### 10、Python 自带的集成开发环境是？（ ） 

A. iPython 

B. Dev-C++ 

C. Visual Studio Code 

D. IDLE 

**参考答案：D** 

在windows电脑的菜单中可以看到。




#### 11、下面哪条语句不能输出：原创精神：自主可控！自主可控！自主可控！（ ） 
A. print('原创精神：自主可控！自主可控！自主可控！') 

B. print('原创精神：' + '自主可控！'*3) 

C. print('原创精神：自主可控！'*3) 

D. print('原创精神：' + '自主可控！' *2 + '自主可控！')



**参考答案：C** 

字符串 `*` 数字，表示重复次数。`+`表示可以将字符串进行相连。

```python
#编程练习
print('原创精神：自主可控！'*3) 
```



#### 12、 在 IDLE 开发环境中，默认是以多少个空格作为代码的基本缩进单位？（

A. 1 

B. 2 

C. 3 

D. 4 



**参考答案：D** 

 Python是以4个空格键为缩进的，也可以用一个`Tab`进行缩进（代表四个空格）







#### 13、 turtle 绘图中，设置画布高度 500 像素，宽度 500 像素，置为（0,0）的代码是（） 

A. turtle.screensize(500,500,0,0) 

B. turtle.screensize(0,0,500,500) 

C. turtle.setup(0,0,500,500) 

D. turtle.setup(500,500,0,0) 



**参考答案：D** 

setup参数的顺序是 width、height、startX、startY

```python
#编程练习
import turtle

turtle.setup(500,500,0,0)
```





#### 14、下列变量名正确的是？（ ） 

A. 54_name

B. name? 

C. _name 

D. 'name' 



**参考答案：C** 

只能用字母或下划线开头，然后可以用字母、数字、`_`。

变量名区分大小写。

```python
#编程练习
_name_345_ = 100
print(_name_345_)

name = 100
Name = 200
print(Name)
print(name)
```



#### 15、想要计算 456 除以 13 的余数，可以使用的符号是？（ ） 

A. * 

B. % 

C. // 

D. # 



**参考答案：B**

A：乘法运算

B：取余数运算

C：整除运算

D：注释符号 

```python
#编程练习
a = 456
b = 13

print(a * b)
# print(a / b)
print(a % b)
print(a // b)
```



#### 16、下列运算符中，优先级最高的是？（ ） 

A. != 

B. and 

C. *= 

D. * 

**参考答案：D** 

```python
#编程练习
a = 456
b = 13
c = 2

c *= a + b
print(c)
```

<img src="https://aimadao.com/static/upload/1568287353733152.png" alt="img" style="zoom:30%;float:left;" />



#### 17、已知变量 a = 7，b = 8，执行语句 a *= a + b 后，变量 a 的值为？（ ） 

A. 15 

B. 22 

C. 8 

D. 105 

**参考答案：D** 

先算 a + b 的结果是 15 ，再用 15 和 a 相乘赋值，得到 15 * 7 = 105

```python
#编程练习
a = 7
b = 8

a *= a + b
print(a)
```



#### 18、关于下面程序，描述正确的是？（ ） 

import turtle 

turtle.goto(100,100) 

turtle.goto(100,-100) 

turtle.goto(-100,-100) 

turtle.goto(-100,100) 

A. 运行代码后，会画出一个正方形。 

B. 运行代码后，会画出一个正方形以及一条从(0, 0)到(100, 100)的连线。 

C. 运行代码后，turtle 面朝方向是水平向右。 

D. 运行代码后，turtle 面朝方向是竖直向上。



**参考答案：C** 

可以根据x、y的坐标画图，然后再判断A、B、C、D。

答案C：turtle并没有用left、right进行自身方向调整，所以turtle自身方向一直是水平向右的。

```python
#编程练习
import turtle

turtle.pensize(3)

turtle.goto(100,100)
turtle.goto(100,-100)
turtle.goto(-100,-100)
turtle.goto(-100,100) 
```





#### 19、运行下列代码，输出区会打印出？（ ） 

```
a = int(3.2) 
print(a) 
```

A. 3 

B. 程序运行错误，没有输出。 

C. 3.3 

D. True 



**参考答案：A** 

小数变成整数，会自动去掉小数点后面所有的数字。

```python
#编程练习
a = int(3.6)
print(a)

b = input("请输入一个数字：")
print(type(b))

c = int(b)
print(c)
```



#### 20、下列关于 python 语言说法正确的是？（ ） 

A. Python 采用代码缩进和冒号':'区分代码之间的层次。 

B. 在 IDLE 编写代码时，使用中文输入代码中的小括号或者双引号，任何位置都不会产生语法错误。 

C. Python 32 位和 64 位的安装包没有区别，可以任意使用一个。 

D. Pycharm 和 Microsoft Visual Studio 都可以用来编写 Python 程序，但是语法和 IDLE 不一致。 



**参考答案：A** 

B：编程中使用英文输入法。

C：不同操作系统选择的Python安装包是不一样的。

D：对于不同的编程工具来说，Python的语法都是一样的。

```python
#编程练习
for i in range(1,10):
    print(i)
```



#### 21、小明家在 A 点的位置，学校在 B 点的位置，如果不绕路，从 A 到 B 的路线共有几条？（ ）

<img src="./imgs/image-20230828165047680.png" alt="image-20230828165047680" style="zoom:30%;float:left;" />

A. 1 

B. 2 

C. 4 

D. 6 

**参考答案：C** 

考察的是数学题：2 * 2 = 4条



#### 22、下列程序的输出结果是？（ ） 

```
a=4 
b=3 
c=2 
print(a*b**c)
```

A. 24 

B. 144 

C. 36 

D. 12 



**参考答案：C**

根据Python运算符的优先级，先算b**c，也就是3的平方，得到的是9；然后再算 4 * 9 ，得到的是 36

```python
#编程练习
a = 4
b = 3
c = 2

print(a * b ** c)
```




#### 23、已知 a=4,b=2,执行语句 a*=a-b 后，变量 a 的值是？（ ） 

A. 8 

B. 2 

C. 14

D. 16 



**参考答案：A** 

根据Python运算符的优先级，先算a-b，得到的是2；然后再算 4 * 2 ，得到的是 8

```python
#编程练习
a = 4
b = 2

a *= a - b
print(a)
```



#### 24、 print(20 or 15<20)的输出结果为？（ 

A. True 

B. False 

C. 20 

D. 15 



**参考答案：C**

在 or 的表达式中，会直接判断 or 前面的是否表达 `True`，如果是，那么or后面的将不会执行。

20 表达的是"真值"，所以直接将20输出了。

```python
#编程练习
print(20 or 15 < 20)
print(-1 or 15 < 20)
print(0 or 15 < 20)
```




#### 25、在式子：2（ ）2；中间括号里填写哪个数学运算符，结果不等于 4？（ ） 

A. // 

B. ** 

C. * 

D. + 



**参考答案：A** 

A是整除，得到的结果是 1 。





### 二、判断题(共 10 题，共 20 分) 



#### 26、then 属于 Python 的保留字。（ ）

A. 正确 

B. 错误 



**参考答案：错误** 

 <img src="https://aimadao.com/static/upload/1562353151770656.png" alt="img" style="zoom:50%;float:left;" />















#### 27、在 Python shell 中输出“Hello，我的新朋友，很高兴认识你！”，正确的语句是 print(Hello，我的新朋友，很高兴认识你！)。（ ） 

A. 正确 

B. 错误 



**参考答案：错误** 





#### 28、在 Python 中，”2022”与 2022 都属于字符串。（ ） 

A. 正确 

B. 错误 



**参考答案：错误** 






#### 29、在 turtle 绘图中，默认的形状是一个小海龟，有些程序完成后需要将小海龟进行隐藏，可以使用 turtle.hideturtle() 指令进行隐藏。（ ） 

A. 正确 

B. 错误 



**参考答案：正确**






#### 30、 如果想要将 a=2 与 b=3 的两个变量赋值写在一行指令中，可以写 a=2;b=3 的格式。（ ） 

A. 正确 

B. 错误 



**参考答案：正确** 





#### 31、 print(type(6/1.8)) 输出结果为<class "float">。（ )

A. 正确 

B. 错误 



**参考答案：正确** 

 



#### 32、运行下面代码，可以在海龟画图窗口上画一个黑色边框，红色填充的圆。（ ） 

```
import turtle 
turtle.penup() 
turtle.begin_fill() 
turtle.color('black', 'red') 
turtle.circle(100) 
turtle.end_fill()
turtle.pendown() 
turtle.forward(100) 
```

A. 正确 

B. 错误 



**参考答案：错误** 

 读源码



#### 33、可以用运算符*连接两个字符串，表示将两个字符串拼接到一起。（ ） 

A. 正确 

B. 错误 



**参考答案：错误** 

 

#### 34、在 Linux 系统上可以运行 python。（ ） 

A. 正确 

B. 错误 



**参考答案：正确** 

 windows、MacOS、Linux 、Unix 都是可以运行python的



#### 35、 Python 启动后显示的提示符是 >>> （ ）

A. 正确

B. 错误 



**参考答案：正确** 

 



### 三、编程题(共 2 题，共 30 分) 



#### 36、每个人都知道自己的鞋码，但是不知道自己的脚长，请写一个程序，帮助大家利用鞋码算出脚长。 



**要求：** 

1.允许用户输入自己的鞋码，并有提示语 '请输入你的鞋码：'，不需要包括单引号； 

2.计算鞋码，脚长 = (鞋码 + 10) / 2； 

3.输出脚长，并有提示语 '你的脚长是(单位:厘米）：'，不需要包括单引号。 



**示例：** 

输入：38 

输出：你的脚长是(单位:厘米）：24.0 



**评分标准：** 

（1）有输入语句；（3 分） 

（2）有输出语句；（1 分） 

（3）有类型转化语句，并且类型转换正确，否则该项分数为 0；（2 分） 

（4）有计算语句，并且计算正确，如果计算错误该项分数为 0；（2 分） 

（5）程序符合题目要求，运行正确。（2 分） 



**参考程序：**

```python
a = input("请输入你的鞋码：")

xie_ma = float(a)

jiao_chang = (xie_ma + 10) / 2

print("你的脚长是(单位:厘米）: %.1f"%jiao_chang)
```






#### 37、按照要求绘制一个五角星。

(1)海龟初始位置的坐标为(0,0)； 

(2)设置画笔大小为 5；

(3)画笔颜色为红色(red)； 

(4)五角星填充颜色为黄色(yellow)。 

(5)五角星大小不限，但是要能清晰看出是五角星，并且完全在考试平台上显示出来。 

<img src="imgs/微信截图_20230912183235.png" alt="微信截图_20230912183235" style="zoom:33%;float:left;" />

**题解**

五边形内角和为540度，那么每个内角是108度；

`right(144)`



**参考程序：** 

```python
import turtle

pen = turtle.Turtle()

pen.pensize(5)
pen.color('red','yellow')

pen.begin_fill()

for i in range(5):
    pen.forward(400)
    pen.right(144)

pen.end_fill()
```



**评分标准：** 

（1）海龟初始位置的坐标为(0,0); (2 分) 

（2）有绘制线条; (2 分) 

（3）画笔颜色设定为红色(red); (2 分) 

（4）画笔大小为 5; (3 分) 

（5）五角星填充颜色为黄色(yellow); (3 分) 

（6）能写出 turtle.left(144)或者 turtle.right(144); (2 分) 

（7）能完全显示在考试平台（2 分） 

（8）画出完整的五角





---



### 附录



#### 1、Turtle函数

Turtle 是 Python 中一个用于绘制图形的库，通常用于教育和初学者学习编程。

Turtle 库提供了一种简单的方式来绘制各种形状和图案，通过移动一只"海龟"（turtle）来控制图形的绘制。

以下是一些常用的 Turtle API 方法和说明：

##### 一、创建 Turtle 对象

- `turtle.Turtle()`: 创建一个新的 Turtle 对象。

##### 二、移动海龟

- `forward(distance)`: 向前移动指定距离。

- `backward(distance)`: 向后移动指定距离。

- `right(angle)`: 右转指定（相对）角度。

- `left(angle)`: 左转指定（相对）角度。

- `seth(angle)`: 左转指定（绝对）角度

- `home() `：初始位置和初始方向。

##### 三、画笔控制

- `penup()`: 抬起画笔，移动时不绘制。

- `pendown()`: 放下画笔，移动时绘制。

- `pensize(width)`: 设置画笔的宽度。

- `pencolor(color)`: 设置画笔的颜色。

##### 四、绘制形状

- `circle(radius)`: 以当前位置为中心绘制一个圆。

- `dot(size)`: 在当前位置绘制一个点。

- `goto(x, y)`: 移动到指定坐标。

- `setx(x)`: 设置 x 坐标。

- `sety(y)`: 设置 y 坐标。

- `setposition(x, y)`: 设置位置坐标。
  

##### 五、颜色控制

- `color(*args)`: 返回或设置画笔颜色和填充颜色。turtle.color("red", "green")

- `fillcolor(color)`: 设置填充颜色。

- `begin_fill()`: 开始填充。

- `end_fill()`: 结束填充。

- `bgcolor(*args)`：设置或返回 TurtleScreen 的背景颜色。screen.bgcolor("orange")

##### 六、清空和控制

- `clear()`: 清空画布。

- `reset()`: 重置海龟位置和状态。

- `hideturtle()`: 隐藏海龟图标。

- `setup`：设置窗口位置和大小，setup (width=200, height=200, startx=0, starty=0)

##### 七、其他方法

- `speed(speed)`: 设置绘制速度。

- `isdown()`: 检查画笔是否放下。

这只是 Turtle 库的一小部分功能，您可以根据需要查阅完整的 Turtle 文档以了解更多详细信息和用法。

官方文档：https://docs.python.org/zh-cn/3/library/turtle.html



##### 八、相对角度和绝对角度

<img src="https://aimadao.com/static/upload/1568259782475808.png" alt="img" style="zoom:33%;float:left;" />

# 一、python语言特点

## 	1.1.  面向对象

* 类别：

  ~~~	python
  class Water:
  	pass
  ~~~

  

## 1.2. 解释型

* 跨平台：(跨操作系统)

  * Windows(开发)---->> linux(运行)
  * python---->> 解释器(python.exe)+lib（内置器)+pip(包管理器: pip.exe)--可扩展性

    * pip

* python是一门解释型的编程语言，因此具有解释型语言的运行机制

* 依赖于环境，安装解释器

## 1.3. 弱类型

* 改变量----声明的变量是什么值就是什么类型

  <img src="C:\Users\22436\AppData\Roaming\Typora\typora-user-images\image-20220717121853749.png" alt="image-20220717121853749" style="zoom: 67%;" />

# 二、 写代码

## 2.1. 步骤 

* 进入环境--》python，终端输入

* python源文件：xxx.py  拓展名是py

  <img src="C:\Users\22436\AppData\Roaming\Typora\typora-user-images\image-20220717134118522.png" alt="image-20220717134118522" style="zoom:50%;" />

## 2.2. 工作原理

<img src="C:\Users\22436\AppData\Roaming\Typora\typora-user-images\image-20220717105701896.png" alt="image-20220717105701896" style="zoom:50%;" />

<img src="C:\Users\22436\AppData\Roaming\Typora\typora-user-images\image-20220717110724946.png" alt="image-20220717110724946" style="zoom:50%;" />



* 交互式 --所见即所得、无法保存；源文件式（sublime）---统一编辑，可长期保存、维护、快速格式化

# 三、变量

## 3.1. 原理

* 变量生活中相当于容器，放东西；编程中也是
* 在python中，变量：内存开辟，声明变量实际是给内存要空间
* 变量中存放的类型：字符串、整型、浮点型、布尔类型、列表、字典

<img src="C:\Users\22436\AppData\Roaming\Typora\typora-user-images\image-20220717120857284.png" alt="image-20220717120857284" style="zoom:50%;" />

* 修改变量 内存空间不变，值改变

  <img src="C:\Users\22436\AppData\Roaming\Typora\typora-user-images\image-20220717121106146.png" alt="image-20220717121106146" style="zoom:50%;" />

## 3.2. 命名原则

* 见名知义

* 由字母、数字、__ 命名，不能以数字开头，不建议中文

  ~~~	python
  name01 ="张三"
  name_01 = "张三"
  __name_01 = "李四"
  01name = "王五" # 错误命名
  name+01 = "张三" # 错误命名
  ~~~

  

  ![image-20220717123835409](C:\Users\22436\AppData\Roaming\Typora\typora-user-images\image-20220717123835409.png)

  

* 严格区分大小写

* 不能以python关键字命名

  * 查看关键字![image-20220717122928760](C:\Users\22436\AppData\Roaming\Typora\typora-user-images\image-20220717122928760.png)

* 建议

  * 驼峰式：由多个单词组成，第一个单词小写，后面每个单词首字母大写

    ​				getName  payMoney getElementsByName

  * 下划线式(推荐)：get_name  goods_total  goods_num

* 定义类名：每个单词首字母大写

* 常量名字大写   NAME=”刘“表示常量

# 四、用法

## 4.1. print

~~~	python
# print(value,value,value...,sep=" ",end="\n")  ---默认每个值后空一格，换行
# print(value,value,value...,sep="# ",end="")---更改为每个值后#号分割，不换行输出
~~~

<img src="C:\Users\22436\AppData\Roaming\Typora\typora-user-images\image-20220717141556374.png" alt="image-20220717141556374" style="zoom:50%;" />

~~~	python
print("亲爱的ki\n     请点击超链接激活用户")
print("亲爱的ki\n","    请点击超链接激活用户")
~~~

<img src="C:\Users\22436\AppData\Roaming\Typora\typora-user-images\image-20220717142332981.png" alt="image-20220717142332981" style="zoom:50%;" />

## 4.2. 转义字符

* \n 换行
* \t 制表符 四空格
* \r 打印头回到行首
  * 补充：

~~~	python
print("乔治说：'想玩恐龙'") 
print('乔治说：\'想吃零食\'')# 转义字符\ \\
print("乔治说：\"想睡觉\"")
print("hello\r hhhh")
print(r"hello\py\\thon") # "r":表示原样输出，不考虑转义字符
print("hello\py\\thon")
~~~

<img src="C:\Users\22436\AppData\Roaming\Typora\typora-user-images\image-20220717152651402.png" alt="image-20220717152651402" style="zoom:50%;" />

## 4.3. 字符串

* 表示：” “    ‘ ’   ”‘ ’‘’
  * ‘’‘ ’‘’适合信息较长的输出，保证原格式输出  ；作为注释使用

~~~	python
print('''
亲爱的刘同学：
	你注册的腾讯视频还未激活，请点击下方链接进行激活，
	请点击：激活用户
	激活用户即可看完整视频。

  from : tengxun team

  	data: 2022/07/17
 ''')
~~~

<img src="C:\Users\22436\AppData\Roaming\Typora\typora-user-images\image-20220717150709622.png" alt="image-20220717150709622" style="zoom:50%;" />

* 格式化输出

~~~	python
name = "姜小君"
age = 20
nation = "中国"
print("我是"+name+",年龄是"+age+",来自"+nation)
# "+"只能拼接字符串 字符串+int类型---》TypeError
# 推荐%s %d %f格式化输出
print("我是%s, 年龄是%s, 来自%s"%(name, age, nation))
~~~


































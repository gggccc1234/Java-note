# Java学习笔记

## 新数据类型
+ byte  -2^7~2^7-1
+ short  -2^15~2^15-1
+ int  -2^31~2^31-1
+ long  -2^63~2^63-1  后缀一定要加L
+ float  8位有效数字  后缀一定要加F
+ double  16位有效数字   后缀可选加D
+ 低精度可以直接赋值给高精度，反之必须使用类型转换运算
+ 对整数使用(char)强制类型转换，数字会变成对应的unicode码对应的字符
+ 数据类型的最大值类似 Integer.MAX_VALUE, 最小值 Integer.MIN_VALUE
## 输入输出数据
+ Scanner 类
+ System.out.print
+ System.out.println  会换行
+ %d
+ %c
+ %f
+ %s
+ %md
+ %m.nd
+ 输入格式类似 C 的printf
## 数组
+ int [] a
+ int a[][]
+ int [] a,b[]  声明了一个一维数组和二维数组
+ 不能直接在中括号内声明数组的长度，使用new声明才可以
+ 与 c 相同，输出char型数组的数组名会输出整个数组的值
## 运算
+ 补码，负数的补码为正数的原码取反后加一
+ 按位与 &
+ 按位或 |
+ 按位非 ~
+ 按位异或 ^
+ a instanceof b b是否是a的祖先
## 面向对象
+ 封装性
+ 继承
+ 多态
+ 成员变量有默认值，局部变量没有
+ 类内变量赋值只能出现在方法体内或在声明的时候赋值
+ UML图
+ 构造方法 类C
+ 类内定义了构造方法，默认构造函数会被覆盖掉
+ 引用类型数据存在栈中，非引用类型数据存在堆中
+ 没有析构函数
+ System.gc() 立即进行垃圾回收
+ 可变对象
+ 关联关系  a类成员变量是b类对象
+ 依赖对象  a类的方法中的参数是b类对象或者方法返回的值是b类对象
+ 实例变量，类变量（static静态变量）
+ 类方法只能由对象调用，只能调用类变量
+ 包名，类似于命名空间，防止变量污染  使用pakeage定义包名
+ import 用于导入别的包里的类
+ java.lang 基本语言类
+ java.io 输入输出类
+ java.util 实用类
+ java.sql 操作数据库的类
+ java.net 实现网络功能的类
+ 引入全部类
+ private 友好 protected public
+ final声明的类不能被继承，声明的变量为常量
+ 上转型对象
+ 继承和多态
+ abstract定义抽象类
+ 开闭原则
+ 静态方法属于类，不可重写，非静态方法属于类的实例，可重写
+ interface 接口体中所有常量的访问权限一定是public,并且是static常量,所有方法的访问权限为public
+ implements 声明实现接口
+ 内部类和外嵌类
+ throws 声明要产生的异常 throw 抛出异常
+ try catch finally
+ assert 断言语句
## String类
+ 可用字符数组的数组名构造String对象
+ .length()
+ .equals()
+ .startsWith()
+ .compareTo()
+ .contains()
+ .substring()
+ .trim()
+ .valueOf()
+ .toString()
+ .getChars()
+ .toCharArray()
## 正则表达式
+ replaceAll返回一个新对象
+ split
## StringTokenizer
+ nextToken()
+ hasMoreTokens()
+ countTokens()
## Scanner
+ next()
+ hasNext()
## StringBuffer
+ append()
+ length()
+ capacity()
+ charAt()
+ setCharAt()
+ insert()
+ reverse()
+ delete()
+ replace()
## Date
## Calendar
+ roll()
+ get()
+ set()
+ String对象的format格式化时间，也可用于格式化数字
## Math
+ random 产生一个0到1之间的随机数，不包括0，1
+ ceil 向上取整，返回一个double型数据
+ floor 向下取整，返回一个double型数据
+ round 四舍五入，返回一个整数
## BigInteger
+ add()
+ subtract()
+ multiply()
+ divide()
+ remainder() 求余
+ compareTo()
+ abs()
+ pow()
+ toString()
## Random
+ nextInt()
+ nextBoolean()
## Class类
## Console类
+ readPassword()
## Pattern
+ complie()
+ matcher()
## Matcher
+ find()  类似js中的lastIndex
+ start()
+ end()
+ group()
+ matches()  判断regex与input是否完全匹配
+ replaceAll()
+ replaceFirst() 只替换查找到的第一个
## runtime
+ freeMemory()
+ totalMemory()
+ getRuntime()
+ exec()
## File
+ getName()
+ canRead()
+ canWrite()
+ exists()
+ length() 单位是字节
+ getAbsolutePath()
+ getParent()
+ isFile()
+ isDirectory()
+ isHidden()
+ lastModified()  最后修改时间
+ mkdir() 创建一个目录
+ list() 返回当前目录下的所有文件，返回字符串数组  可以传入FilenameFilter,返回指定的后缀
+ listFiles() 返回files数组
+ delete()
## FileInputStream
+ read()
+ close()
## FileOutputStream
+ 构造函数的append参数，if true 写入文件追加到原文件后面，else false 原文件被刷新
+ write()
+ close()
## FileReader, FileWriter
+ 先把数据写到缓冲区，每当缓冲区溢出，溢出的数据被自动写入到目的地，可用flush()清洗缓冲区
## BufferedReader, BufferedWriter
+ readLine() 读入一行
+ newLine() 写入一个换行符
## 随机流 RandomAccessFile
+ 构造函数参数 mode r只读，rw可读写
+ 不刷新文件
+ colse, read, write
+ getFilePointer() 获取当前读写位置
+ seek 定位读写位置
## 数组流
## 数据流





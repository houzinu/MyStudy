# 数组

  ### 4. 内存分配

###### 4.1 Java中内存分配

![image-20220720221617517](C:\Users\yangc\AppData\Roaming\Typora\typora-user-images\image-20220720221617517.png)

数组在初始化时，会为存储空间添加默认值

* 整数：0（默认值）
* 浮点数：0.0
* 布尔值：false
* 字符:空字符
* 引用数据类型：null

###### 数组内存图（多个数组）

![image-20220721085329056](C:\Users\yangc\AppData\Roaming\Typora\typora-user-images\image-20220721085329056.png)

数组操作的时候有两个问题

1. 索引越界；---访问了数组中不存在的索引对应的元素。
2. 空指针异常。---访问的数组已经不再指向堆内存的数据。

###### 获取数组元素量

==格式==：数组名.length

==范例==：arr.length

# 5. 方法（method）

### 方法的定义和调用

格式： public static void 方法名( ){

​				//方法体

}

**方法的调用**： 方法名（ ）；

​			范例：isEvenNumber( );

### 带参数方法的定义和调用

格式： public static void 方法名（参数）{ }

​             public static void 方法名 （数据类型 参数，数据类型2 参数2，...){};

### 带返回值方法的定义和调用

public static boolean isEvenNumber (int number)

{

return true;

}

调用：boolean flage = isEvenNumber(5);

==分法不能嵌套定义==

### 方法名重载

方法名相同，参数不同；

### this  关键字

this修饰的name是成员变量的name，不是局部变量的name。

# String

# StringBulider

StringBulider是一个空白的可变字符串对象，里边不含有任何内容

![image-20220722125125149](C:\Users\yangc\AppData\Roaming\Typora\typora-user-images\image-20220722125125149.png)



![image-20220722140645611](C:\Users\yangc\AppData\Roaming\Typora\typora-user-images\image-20220722140645611.png)

# static

用Static修饰符修饰的变量———可以被类的所有成员共享。

# 多态

多态中成员访问的特点：

成员变量：编译看左，执行看左

成员方法：编译看左，执行看右

（因为成员方法有重写而成员变量没有）。

# 接口（interface)

接口成员的特点：

* 成员变量
  * 只能是常量；默认修饰符：public static final
* 构造方法
  * 接口没有构造方法，因为接口主要是对行为进行抽象的，是没有具体存在
  * 一个==类==如果没有==父类==，默认继承自Object类
* 成员方法
  * 只能是抽象方法；默认修饰符：public abstract

# 形参和返回值

###### 类名作为形参和返回值

方法的形参是类名，其实需要的是该类的对象

方法的返回值是类名，其实返回的是该类的对象

###### 抽象类作为形参和返回值

方法的形参是抽象类名，其实需要的是该抽象类的子类对象

方法的返回值是抽象类名，其实返回的是该抽象类的子类对象

###### 接口名作为形参和返回值

方法的形参是接口名，其实需要的是该接口的实现类对象

方法的返回值是接口名，其实返回的是该接口的实现类对象

# 内部类

###### 内部类的访问特点

内部类可以直接访问外部类的成员，包括私有

外部类要访问==内部类==的成员，必须创建对象

###### 局部内部类

局部内部类是在方法中定义的类，所以外界是无法直接使用，需要在方法内部创建对象并使用

该类可以直接访问外部类的成员，也可以访问方法内的局部变量。






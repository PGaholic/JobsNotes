# Java 面试准备

注：资源来自互联网，如有侵权请联系1697200598@qq.com删除。

<!-- TOC -->

- [Java 面试准备](#java-面试准备)
    - [Java 基础](#java-基础)
        - [面向对象基本特征](#面向对象基本特征)
        - [final，finally，finalize的区别](#finalfinallyfinalize的区别)
        - [int 和 Integer 有什么区别](#int-和-integer-有什么区别)

<!-- /TOC -->

## Java 基础

### 面向对象基本特征
  * 继承
  * 抽象
  * 多态
  * 封装

### final，finally，finalize的区别
  final为修饰关键字，能够修饰变量、方法、类。被final修饰的类，就意味着不能再派生出新的子类，不能作为父类而被子类继承。因此一个类不能既被abstract声明，又被final声明。将变量或方法声明为final，可以保证他们在使用的过程中不被修改。被声明为final的变量必须在声明时给出变量的初始值，而在以后的引用中只能读取。被final声明的方法也同样只能使用，即不能方法重写。

  finally为异常处理提供finally块执行清楚操作，不管有没有异常被抛出、捕获，finally块都会被执行。
  
  finalize是方法名。Java技术允许使用finalize()方法在垃圾收集器将对象从内存中清理出去之前做必要的清理工作。这个方法是由垃圾收集器在确定这个对象没有被引用时对这个对象调用的。它是在object类中定义的，因此所有的类都继承了它。子类覆盖finalize（）方法以整理系统资源或者被执行其他清理工作。在垃圾回收之前调用。

### int 和 Integer 有什么区别
  int 是基本数据类型
  Integer 是基础类,是int的包装类 
  注意自动拆箱和装箱

  （1）Integer是int的包装类；int是基本数据类型； 
  （2）Integer变量必须实例化后才能使用；int变量不需要； 
  （3）Integer实际是对象的引用，指向此new的Integer对象；int是直接存储数据值 ； 
  （4）Integer的默认值是null；int的默认值是0。

  int与Integer比较的时候，Integer会自动拆箱变成int

  [参考blog](https://blog.csdn.net/chenliguan/article/details/53888018)
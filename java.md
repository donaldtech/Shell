## JDK
```
JDK>JRE>JVM实例
Oracle JDK 8 / OpenJDK 8 / IBM J9 JDK 8
下载 
https://www.oracle.com/technetwork/java/javase/downloads/index.html


安装 
windows
默认
环境变量 Control Panel\System and Security\System\Advanced System Setting\Enviroment Variables\
JAVA_HOME=C:\Program Files\Java\jdk-12
Path=C:\Program Files\Java\jdk-12\bin
验证 cmd: javac -version


目录结构
bin-可执行命令
  javac-Java编译器
  java-运行编译后的JVM应用程序，即使这种程序不是使用Java写的
  桌面GUI监视工具
     jvisualvm  from http://visualvm.github.io/
     jmc
include-供C语言编译器使用的头文件
lib-库
```

## 用包组织类
```
同一包中的类构成了一个命名空间
包         包中的类
basket     Basket,BasketLine-describe sth
product    Product
com.example.jvm_university.webprogramming

package com.example.jvm_university.webprogramming;
class Application {
}
全限定类名com.example.jvm_university.webprogramming.Application
````

## 类库=API
```
类库中的所有类放在包（java...  javax.... org.xml com.oracle...）中
包               类库中的类
java.lang        String, StringBuilder, Object
java.io/net/nio  操作系统，文件，网络IO的类
java/javax.sql   访问JDBC的类

java.lang包
java,lang.Object类

java.lang.String类
java.lang.Number

java.lang.Exception
java.lang.Error

java.util.ArrayList
java.util.HashMap
```


## 第一个java程序
vim HelloWorld.java(文件名需与类名一致)
```
public class HelloWorld {  
    public static void main(String[] args) { //主方法入口：所有的 Java 程序由 public static void main(String []args) 方法开始执行
        System.out.println("Hello World");
    }
}

## 定义包和类
将类放入包中
访问控制	private私有的 / protected受保护的 / public公共的
非访问控制 final最终的，禁止其他类继承
类名大大大
package com.example.package_name;
public final calss ThisIsTheFirstClass {
  访问控制	private私有的 / protected受保护的 / public公共的
  static静态的，没有类的实例也能访问
  final,不能重写；作用于变量时，变量成了常量
  public static String staticVaribale = "haha";
  public final static String STATICVARIABLE = "xixi";
  
  
  可定义方法的不同版本
  
  构造函数，创建类的时候被调用，命名于类相同
  public class ClassWithConstructor {
      public ClassWithConstructor(int a, int b) {
      }
  }
  默认隐式生产构造函数
      public ClassWithConstructor() { }
      
      
  终结方法finalize()在对象被垃圾收集器收集时被JVM调用
}

#### 继承扩展类
class ParentClass {
  void aMethod() {
  }
}

class SubClass extends ParentClass {
  访问父类成员，用super
  super.aMethod();
}

#### 抽象类可以被扩展，不能实例化
public abstarct class AbstartcClass {
  abstract public void aMethod();
}

#### 接口
interface Interface1 {
  void method1();
}

## 导入类
1.全限定类名
java.util.ArrayList list = new java.util.ArrayList();

2.import java.util.ArrayList;
ArrayList list = new ArrayList();

ClassWithConstructor example = new ClassWithConstructor(1,2);  //使用构造函数




$ javac HelloWorld.java   将 java 源文件编译为 class 字节码文件 (HelloWorld.class)
$ java HelloWorld  java文件中的类名
```

## 基础语法
### 对象和类
```
类
public class Dog{
  String breed;
  int age;
  String color;
  void barking(){
  }
 
  void hungry(){
  }
 
  void sleeping(){
  }
}
```
### 基本数据类型
### 变量类型
### 修饰符
### 运算符
### 循环结构
### 条件语句
### switch case
### Number Math类
### Character类
### String类
### StringBuffer
### 数组
### 日期时间
### 正则表达式
### 方法
### Stream File IO
### Scanner类
### 异常处理
## 面向对象

## 高级编程

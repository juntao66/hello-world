#Java学习笔记
```java
public class Hello{
    public static void main(String args[]){
	    System.out.println("hello word")
	}
}
```
##执行该程序
1. 编译源代码文件，形成Hello.class文件
2. 解释Java程序

##程序类的定义
- 类是Java中的基本单位
- public class 类名称{}:文件名称必需与类名称保持一致
- class 类名称{}：文件名称可以与类名称不同  在一个Java文件里可以使用class定义多个类，并且编译后形成不同class文件
**进行类名称定义的时候，要求：每一个单词的首字母要大写 TestDemo**

###主方法：是程序的起点
```
public static void main(String args[]){
	    主方法中编写的代码才是整个程序执行的逻辑
	}
```
**主方法所在的类称为主类**

###信息输出
- 输出后换行：*System.out.println("hello word")*
- 输出后不换行：*System.out.print("hello word")*
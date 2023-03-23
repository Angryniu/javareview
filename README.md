# javareview
# 复习java基础

# 一、配置环境变量（省略）与基础指令
1. 编译代码：java xxx.java
2. 运行代码：java xxx
3. 编码问题使用：javac -encoding UTF-8 xxx.java

# 二、基础语法
## （一）注意事项
1. 大小写敏感
2. 类名通常首字符大写
3. 方法名使用小驼峰
4. 源文件名与类名相同
5. 主方法入口：所有的 Java 程序由 public static void main(String[] args) 方法开始执行

## （二）标识符
1. 首字母以字母（A-Z 或者 a-z）,美元符（$）、或者下划线（_）开始
2. 之后可以是字母（A-Z 或者 a-z）,美元符（$）、下划线（_）或数字的任何字符组合（**不能以数字开头**）

## （三）修饰符
1. 访问控制修饰符 : default, public , protected, private
2. 非访问控制修饰符 : final, abstract, static, synchronized

## （四）Java变量
1. 局部变量:在方法、构造方法或者语句块中定义的变量被称为局部变量。变量声明和初始化都是在方法中，方法结束后，变量就会自动销毁。
2. 类变量（静态变量）:类变量也声明在类中，方法体之外，但必须声明为 static 类型。
3. 成员变量（非静态变量）:成员变量是定义在类中，方法体之外的变量。这种变量在创建对象的时候实例化。**成员变量可以被类中方法、构造方法和特定类的语句块访问**

## （五）Java数组

## （六）Java枚举（限制变量只能使用规定的值，减少bug出现）

## （七）Java关键词
![alt Java关键词](https://github.com/Angryniu/javareview/blob/main/java%E5%85%B3%E9%94%AE%E5%AD%97.png)

## （八）Java注释
```
/*
*多行注释
*多行注释
*/
```
```
//单行注释
/*单行注释*/
```

## （九）继承：利用继承的方法，可以重用已存在类的方法和属性，而不用重写这些代码。被继承的类称为超类（super class），派生类称为子类（sub class）

## （十）接口：接口只定义派生要用到的方法，但是方法的具体实现完全取决于派生类（实现类）

# 三、对象和类
## （一）面向对象的基本概念
1. 多态
2. 继承
3. 封装
4. 抽象
5. 类：类是一个模板，它描述一类对象的行为和状态
6. 对象：对象是类的一个实例
7. 实例
8. 重载
   
### 创建一个类
```java
public class Dog{
    String breed;
    String color;
    int age;
    /*
    *每个类都有构造方法。如果没有显式地为类定义构造方法，Java 编译器将会为该类提供一个默认构造方法。
    *在创建一个对象的时候，至少要调用一个构造方法。构造方法的名称必须与类同名，一个类可以有多个构造方法。
    */
    public Dog(String bread,String color,int age){ 
        this.breed = breed;
        this.color = color;
        this.age = age;
    }
    void eat(){}
    void run(){}
    void sleep(){}
}
```

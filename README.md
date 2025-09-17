# Java_Hero Mastering Object-Oriented Programming in Java
<div style="display:flex">
<img src="https://img.shields.io/badge/Windows_11-0078d4?style=for-the-badge&logo=windows-11&logoColor=white">
<img src="https://img.shields.io/badge/W3Schools-04AA6D?style=for-the-badge&logo=W3Schools&logoColor=white">
<img src="https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=Oracle&logoColor=white">
<img src="https://github.com/Asifekhlaque/Java_Hero/assets/132199879/bb185c13-5a63-4a96-b787-78f6bbbb95be" style="width:50px">
<img src="https://github.com/Asifekhlaque/Java_Hero/assets/132199879/b8e5d917-44f9-45fe-99b1-86de25c1c0a6" style="width:50px;"> 
<img src="https://github.com/Asifekhlaque/Java_Hero/assets/132199879/0a0df93a-d4d8-4ea0-bb29-b851dd4cea4b" style="width:50px;">
</div>
<h1>Basic OOPs</h1>
Its is concept of Object Oriented Programming in Java Language which is uses classes and objects to perform a real life tasks.
<h2>What is Object Oriented Programming in Java?</h2>
<u>
  <li>Object Oriented Programming is a programming paradigm that provides a means of structuring programs so that they are easier to understand, maintain, and debug.</li>
  <li>It's also helps in achieving data hiding and data encapsulation.</li>
</u>
<h2>Advantages of Object Oriented Programming in Java?</h2>
<ul>
  <li>Easy to understand</li>
   <li>Easy to maintain</li>
   <li>Easy to debug</li>
   <li>Reusability</li>
  <li>Encapsulation</li>
  <li>Data hiding</li>
  <li>Flexibility</li>
</ul>
<h2>Disadvantages of Object Oriented Programming in Java?</h2>
Complexity
<h2>Example of Language which supports Object Oriented Programming </h2>
C++,Java,Python,C#,JavaScript,PHP,Ruby,Swift,Kotlin,Go,Dart,Rust
<h2>Conclusion</h2>
Object Oriented Programming is a programming paradigm that provides a means of structuring programs so that they are easier to understand, maintain, and debug.
<h3>Example<h3>
```
  
     public class BasicOOPs {
       void sum(int a, int b){
        int sum = a + b;
        System.out.println(sum);
    }

    public static void main(String[] args) {
        BasicOOPs obj = new BasicOOPs();
        obj.sum(10, 20);
     }
    } 
```
# 4 main pillar of OOPS
<ol>
  <li>Inheritance</li>
  <li>Polymorphism</li>
  <li>Encapsulation</li>
  <li>Abstraction</li>
</ol>
<h1>What is constructor?</h1>
<ul>
  <li>Constructor is a special type of method that is used to initialize objects.</li>
  <li>It not return any value.</li>
</ul>

    public class constructorlearn {
    constructorlearn(){ //! constructor
        System.out.println("I am constructor");
    };
    public static void main(String[] args) {
        constructorlearn obj = new constructorlearn();
        System.out.println("I am main");
     }
    }

<h1>What is this( )?</h1>
<u>
  <li>The this keyword refers to the current object.</li>
  <li>It also call constructor</li>
  <li>It is used to access the members of the current class.</li>
</u>

    public class thisKeyWord {
    int a;
    int b;
    void sum(int a, int b){
        this.a = a;
        this.b = b;
        int sum = a + b;
        System.out.println("this a = "+a+" this b = "+b+" sum = "+sum);
        
    }
    public static void main(String[] args) {
        thisKeyWord obj = new thisKeyWord();
        obj.sum(10, 20);
     }
    }

    //! Note :
    // This can call other constructor through this keyword , so we have to use this().
    public class thisPracticSet {
    int eid;
    String ename;
    double salary;
        thisPracticSet(){ //! default constructor
        this("Rahul",2500.00);
        eid=100;
        System.out.println(eid);
    }
        thisPracticSet(int id){ //! parameterized constructor
        this();
        eid=id;
     }
        thisPracticSet(String ename,double sal){ //! parameterized constructor
        this.ename=ename;
        salary=sal;
        System.out.println(ename+" "+salary);
     }
    public static void main(String[] args) {
        //!new thisPracticSet();
        new thisPracticSet(100);
     }
    }

# What is inheritance?
Inheritance is a mechanism in which one class acquires the properties of another class.
<h2>Types of Inheritance in java</h2>
<ul>
  <li>Single Inheritance: A class inherits from another class.</li>
  <li>Multilevel Inheritance: A class inherits from another class, which in turn inherits from another class.</li>
</ul>

<h2>Use of Inheritance</h2>
<ul>
  <li>Code Reusability</li>
  <li>Code Redundancy</li>
  <li>Extensibility</li>
  <li> Maintainability</li>
  <li>Flexibility</li>
</ul>
Java not support multiple inheritance because of ambiguity or Diamand problem .

Inheritance is a mechanism in which one class acquires the properties of another class.
       
    class A{
    int a=10;
    A(){
        System.out.println("I am A "+a);
        System.out.println("I am constructor of A");
    }
    void display(){
        System.out.println("I am display of A and it is inherited from A");
    }
    void sum(int a, int b){
        int sum = a + b;
        System.out.println(sum);
    }
    }
    public class inheritanceoops extends A{
    public static void main(String[] args) {
        inheritanceoops obj = new inheritanceoops();
        obj.display();
        obj.sum(70, 20);
        System.out.println(obj.a);
    }
    }
# Polymorphism
Polymorphism is the ability of an object to take on many forms.
<br>
Two type of Polymorphism are:
<ol>
  <li>Dynamic Polymorphism (Compile time Polymorphism)</li>
  <li>Static Polymorphism (Run time Polymorphism)</li>
</ol>
<h2>What is dynamic method dispatch?</h2>  
Dynamic method dispatch is a feature of Java that allows you to call a method based on the type of the object on which it is invoked.
<h2>Why it is used?</h2>
It is used to call a method based on the type of the object on which it is invoked.
<h2>Advantages of dynamic method dispatch:</h2>
<ul>
  <li>It allows for polymorphism, where a subclass object can be treated as an instance of its superclass.</li>
  <li>It enables code reusability and flexibility, as different subclasses can have their own implementations of the same method.</li>
  <li>It promotes code organization and maintainability, as related methods can be grouped together in a superclass and overridden in subclasses.</li>
</ul>

    class phone{
    void call(){
        System.out.println("Phone is calling");
    }
    void photo(){
        System.out.println("Phone is taking photo");
    }
    }

    class SmartPhone extends phone{
    @Override
    void call(){
        System.out.println("SmartPhone is calling");
    }
    void sms(){
        System.out.println("SmartPhone is sending sms");
    }
    void play(){
        System.out.println("SmartPhone is playing");
    }
    void Internet(){
        System.out.println("SmartPhone is Internet");
    }
    }

    public class DynamicMethodDispatch {
    public static void main(String[] args) {
        phone obj = new SmartPhone();
        obj.call(); //todo SmartPhone is calling
        obj.photo();
        //! obj.play(); Not allowed
        //! obj.sms(); Not allowed
        //! obj.Internet(); Not allowed`
    }
    }



# Overloading in Java
<ul>
  <li>It is used to achieve reusability.</li>
  <li>The name of the method should be same.</li>
  <li>The number of parameters should be different.</li>
  <li>It is used to achieve polymorphism.</li>
</ul>

# Overriding in Java
<ul>
  <li>It is used to achieve reusability.</li>
  <li>The name of the method should be same.</li>
  <li>The number of parameters should be same.</li>
  <li>It is used to achieve polymorphism.</li>
  <li>It is used to achieve security.</li>
</ul>

    public class overloading_overriding {
     public static void main(String[] args) {
        G a = new G();
        a.Method(); //! Overloading
        a.Method(10); //! Overloading
        F b = new F();
        b.Method(); //! Overriding
        b.Method(10); //! Overriding
     }
    }
    class G{
     void Method(){
        System.out.println("Overloading");
     }
     void Method(int a){//! Overloading
        System.out.println("Overloading");
     }
    }
    class F extends G{
     @Override
     void Method(int a){//! Overriding
        System.out.println("Overriding");
     }
     @Override
     void Method(){ //! Overriding
        System.out.println("Overriding");
     }
    }
# Access Modifier 

<table style="width:100%;border:2px solid ;">
  <tr>
    <th>Modifier</th>
    <th>Class</th>
    <th>Package</th>
    <th>Subclass</th>
    <th>World</th>
  </tr>
  <tr>
    <td>public</td> 
    <td>Y</td>
    <td>Y</td>
    <td>Y</td>
    <td>Y</td>
  </tr>
  <tr>
    <td>protected</td>
    <td>Y</td>
    <td>Y</td>
    <td>Y</td>
    <td>N</td>
  </tr>
  <tr>
    <td>Default(No)</td>
    <td>Y</td>
    <td>Y</td>
    <td>N</td>
    <td>N</td>
  </tr>
  <tr>
    <td>private</td>
    <td>Y</td>
    <td>N</td>
    <td>N</td>
    <td>N</td>
  </tr>
</table>

    public class accesModifer {
      public void display(){
        System.out.println("I am public");
     }
    }
    private class mat{
      private void display(){
        System.out.println("I am private");
     }
    }
    protected class eng{
      protected void display(){
        System.out.println("I am protected");
     }
    }
    
# Abstraction
Abstraction is a process of hiding the implementation details and showing only the functionality to the user.
<br>
Abstraction having two comportant:
<ol>
  <li>Abstract class</li>
  <li>Interface</li>
</ol>

# What is abstract class?
<ul>
  <li>An abstract class is a class that contains one or more abstract methods.</li>
  <li>An abstract method is a method that is declared without an implementation.</li>
  <li>An abstract class cannot be instantiated.</li>
  <li>An abstract class can have abstract methods and non-abstract methods.</li>
</ul>

# Use and Advantage abstract class?
It provide security to your code.

    abstract class Animal{ //todo abstract class
     abstract void eat();
     abstract void play();
     void sleep(){
      System.out.println("Animal is sleeping");
     }
    }
    public class abstractMathod extends Animal{
      void eat(){
            System.out.println("Animal is eating");
      }
      void play(){
            System.out.println("Animal is playing");
      }
      public static void main(String[] args) {
            Animal obj = new abstractMathod();
            obj.eat();
            obj.sleep();
            obj.play();
      }
    }
# What is Interface? 
<ul>
  <li>Interface is a blueprint of a class.</li>
  <li>Interface is used to achieve abstraction.</li>
  <li>Interface is used to achieve reusability.</li>
  <li>Interface is used to achieve polymorphism.</li>
  <li>Interface is used to achieve security.</li>
  <li>We can not create an object of an interface. But we can create a reference of an interface.</li>
  <li>And the properties of an interface are Public by default.</li>
</ul>

# Advantages of Interface?
<ul>
  <li>Better way of defining methods.</li>
  <li>It supports multiple inheritance.</li>
  <li>It is used to achieve data hiding.</li>
</ul>

# Most Most Important thing about Interface
<ol>
  <li>It allow <b>Multi inhertance</b>. Means one class use multiple interface at the same time</li>
  <li>Use Interface we use <b>implements</b> keyword.</li>
</ol>

    interface Bicycle{
     void applyBrake(int decrement);
     void speedUp(int increment);
    }
    class MountainBike implements Bicycle{
      public void applyBrake(int decrement){ //! Method Overriding
        System.out.println("Applying Brake");
      }
      public void speedUp(int increment){
        System.out.println("Speeding up");
     }
     public static void main(String[] args) {
        MountainBike obj = new MountainBike();
        obj.applyBrake(1);
        obj.speedUp(2);
     }
    }

# What is Encapsulation?
Encapsulation is used to achieve data hiding and achieve security.

    public class encapsulation {
    private int a;
    private int b;
    public int getA(){
        return a;
    }
    public int getB(){
        return b;
    }
    public void setA(int a){
        this.a = a;
    }
    public void setB(int b){
        this.b = b;
    }
    public static void main(String[] args) {
        encapsulation obj = new encapsulation();
        obj.setA(10);
        obj.setB(20);
        System.out.println(obj.getA());
        System.out.println(obj.getB());
      }
    }

## Exception Handling
Exception is an unwanted or unexpected event, which occurs during the execution of a program, i.e. at run time
### Checked Exceptions
Checked exceptions are called compile-time exceptions because these exceptions are checked at compile-time by the compiler.
### Unchecked Exceptions
The unchecked exceptions are just opposite to the checked exceptions.

## Array Deque
- Array Deque is used to add or remove elements from both ends.
- It is used to achieve efficient insertion and deletion
```java
import java.util.ArrayDeque;
public class arradeq {
    public static void main(String[] args) {
                // Create an ArrayDeque
                ArrayDeque<Integer> deque = new ArrayDeque<>();

                // Add elements to the front of the deque
                deque.addFirst(1);
                deque.addFirst(2);
                deque.addFirst(3);

                // Add elements to the end of the deque
                deque.addLast(4);
                deque.addLast(5);
                deque.addLast(6);

                // Remove elements from the front of the deque
                int firstElement = deque.removeFirst();
                System.out.println("Removed first element: " + firstElement);

                // Remove elements from the end of the deque
                int lastElement = deque.removeLast();
                System.out.println("Removed last element: " + lastElement);
            }
        }
```

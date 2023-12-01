# Java_Hero
<h1>Basic OOPs</h1>
Its is concept of Object Oriented Programming in Java Language which is used to create classes and objects.
<h2>What is Object Oriented Programming in Java?</h2>
<u>
  <li>Object Oriented Programming is a programming paradigm that provides a means of structuring programs so that they are easier to understand, maintain, and debug.</li>
  <li>It's also helps in achieving data hiding and data encapsulation.</li>
</u>
<h2>Advantages of Object Oriented Programming in Java?</h2>
<u>
  <li>Easy to understand</li>
   <li>Easy to maintain</li>
   <li>Easy to debug</li>
   <li>Reusability</li>
  <li>Encapsulation</li>
  <li>Data hiding</li>
  <li>Flexibility</li>
</u>
<h2>Disadvantages of Object Oriented Programming in Java?</h2>
Complexity
<h2>Example of Language which supports Object Oriented Programming </h2>
C++,Java,Python,C#,JavaScript,PHP,Ruby,Swift,Kotlin,Go,Dart,Rust
<h2>Conclusion</h2>
Object Oriented Programming is a programming paradigm that provides a means of structuring programs so that they are easier to understand, maintain, and debug.
<h3>Example<h3>
     
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

<h1>What is this?</h1>
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
  <li></li>
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

<h2>what is dynamic method dispatch?</h2>  
Dynamic method dispatch is a feature of Java that allows you to call a method based on the type of the object on which it is invoked.
<h2>why it is used?</h2>
It is used to call a method based on the type of the object on which it is invoked.
<h2>Advantages of dynamic method dispatch:</h2>
<ul>
  <li>It allows for polymorphism, where a subclass object can be treated as an instance of its superclass.</li>
  <li>It enables code reusability and flexibility, as different subclasses can have their own implementations of the same method.</li>
  <li>It promotes code organization and maintainability, as related methods can be grouped together in a superclass and overridden in subclasses.</li>
</ul>

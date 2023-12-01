# <h1 style="color:red">Java_Hero</style>
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

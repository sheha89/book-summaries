Head First Java 2nd Edition
===========================

This is a repository for the following tutorials Head First Java by Kathy Sierra and Bert Bates.

Chapters
-
1. [Chapter 01](src/head/first/java/chapter01/Chapter01.md)
2. [Chapter 02](src/head/first/java/chapter02/Readme.md)
3. [Chapter 03](src/head/first/java/chapter03/Readme.md)
4. [Chapter 04](src/head/first/java/chapter04/Readme.md)
5. [Chapter 05](src/head/first/java/chapter05/Readme.md)
6. [Chapter 06](src/head/first/java/chapter06/Readme.md)
7. [Chapter 07](src/head/first/java/chapter07/Readme.md)
8. [Chapter 08](src/head/first/java/chapter08/Readme.md)
9. [Chapter 09](src/head/first/java/chapter09/Readme.md)
10. [Chapter 10](src/head/first/java/chapter10/Readme.md)
11. [Chapter 11](src/head/first/java/chapter11/Readme.md)
12. [Chapter 12](src/head/first/java/chapter12/Readme.md)
13. [Chapter 13](src/head/first/java/chapter13/Readme.md)
14. [Chapter 14](src/head/first/java/chapter14/Readme.md)
15. [Chapter 15](src/head/first/java/chapter15/Readme.md)
16. [Chapter 16](src/head/first/java/chapter16/Readme.md)
17. [Chapter 17](src/head/first/java/chapter17/Readme.md)


Head First Java Chapter 01
=====

Bullet Point.
--
* The **assignment** operator uses *_one_* equals sign **=**.  
* The **equals** operator uses *_two_* equals sign **==**.
* A *while* loops runs everything within its block, as long as the *conditional* test is **true**.
* If the *conditional* is **false**, the while loop code block won't run, and execution will move to the code immediately *after* the loop block.



Head First Java Chapter 02
=====
This is the second Chapter learning of **Head First Java** by **Kathy Sierra** and **Bert Bates**, 
This markdown file is my notes for the second chapter, not sure if any copyright issues are there.

Procedural Programmer (PP) vs Object Oriented Programmer(OOP)
-
* PP thinks in terms of what things this program has to *do*, but OOP thinks what are the **things** in the program.
* When Specification of program change the PP have to change the existing code and re-test all, but for OOP, he has
test only the changed portion.
* In OO programming, you can always follow these steps for efficient design
 * Check what is common in all the classes.
 * Abstract the common feature and put in a super class.
 * Inherit all the Sub Class with feature from Super class.
 * Override any specific requirement in one of the Sub Class.

Bullet Point
--
* Object-Oriented programming lets you extend a program without having to touch previously-tested, working code.
* All java code is defined in a **class**.
* A class describes how to make an object of that class type. **A Class is like a blueprint.**
* An object can take care of itself, you don't have to know or care *how* the object does it.
* An object **knows** things and **does** things.
* Things an object knows about itself are called **instance variables**. They represent the *state* of an object.
* Things an object does are called **methods**. They represent the *behavior* of an object.
* When you create a class, you may also want to create a separate test class which you will use to create objects of your class type.
* A class can **inherit** instance variables and method from a more abstract **superclass**.
* At runtime, a java program is nothing more than objects 'talking' to other object.
 


 Head First Java Chapter 03
=====
This is the third Chapter learning of **Head First Java** by **Kathy Sierra** and **Bert Bates**, 
This markdown file is my notes for the third chapter, not sure if any copyright issues are there.


###Declaring a variable
* **Java cares about type.**, So for this **type safety** to work, you must declare the type of your variable.  
**Variables** are of two type:  
1 **Primitive**  
2 **Object Reference**

There is only these two declaration rule.  
1 **variables must have a type.**  
2 **variables must have a name.**  

####Primitive Type
| Type          | Bit Depth     | Value Range  |
| ------------- |:-------------:| :-----:|
| **boolean**| JVM Specific|true/false |
| **char**| 16 bits|0 to 65535 |
| **byte**| 8 bits|-128 to 127 |
| **short**|16 bits| -32768 to 32767|
| **int**| 32 bits | -2147483648 to 2147483647|
| **long**|64 bits | huge|
|**float**|32 bits | varies|
|**double**|64 bits | varies|

There are eight primitive types:  
    **b**oolean **c**har **b**yte **s**hort **i**nt **l**ong **f**loat **d**ouble  
you can remember it like,  
    **b**e **c**arefull **b**ears **s**houldn't **i**ngest **l**arge **f**urry **d**og

* You can put a very large value say(long) into a small value(int), without losing information
* But you can put small value in a large variable.

####Primitive Naming Convention.
Here is the rules for naming a variables.  
1. **It must start with a letter, underscore(_), or dollar sign ($). You can't start a name with a number.**  
2. **After the first character, you can use numbers as well, just don't start it with a number.**  
3. **It cannot be from the Java reserved words.**  

####Object Reference
* There is actually no such thing as an object variable.  
* There's only an object reference variable.
* An Object reference variable holds bits that represent a way to access an object.
* It doesn't hold the object itself.
* **Object reference are like Remote Control for actual object.**
* You cannot do arithmetic on a reference variable.

####Array
* Declare an int array variable, An array variable is a remote control to an array object.

````java
int[] nums
````
* Create a new int array with a length of 3.  

````java
nums = new int[3]
````
* Give each element in the array an int value.  

````java
nums[0] = 6;
nums[1] = 5;
nums[2] = 4;
````
* Arrays are always objects, whether they're declared to hold primitives or object reference.  
* Once you've declared an array, you can't put anything in it except things that are of the declared type.  

Bullet Point
--
* Variables come in two flavors: primitive and reference
* Variable must always be declared with a name and a type.
* A primitive variable value is the bits representing the value (5, 'a',true, etc)
* A reference variable value is the bits representing a way to get to an object on the heap.
* A reference variable is like a remote control, using the dot operator (.) on a reference variable is like pressing a button on the remote control to a access a method or instance variable.
* A reference variable has a value of *null* when it is not referencing any object.
* An array is always an object, even if the array is declared to hold primitives.    

						

Head First Java Chapter 04
=====
This is the fourth Chapter learning of **Head First Java** by **Kathy Sierra** and **Bert Bates**, 
This markdown file is my notes for the fourth chapter, not sure if any copyright issues are there.

Bullet Points
-

* Classes define what an object knows and what an object does.
* Things an object knows are its **instance variable**.
* Things an object does are its **method**.
* Methods can use instance variables so that objects of the same type can behave differently.
* A method can have parameters, which means you can pass one or more values into the method.
* The number and type of values you pass in must match the order and type of the parameters declared by the method.
* Values passed in and out of methods can be implicitly promoted to a larger type or explicitly cast to a smaller type.
* The values you pass as an arguments to a method can be a literal value or a variable of the declared parameter type.
* A method must declare a return type, A void return type means the method doesn't return anything.
* if a method declares a non-void return type, it must return a value compatible with the declared return type.

###Encapsulation.
* To support encapsulation, the instance variable should be hidden by the use of **private** access modifiers.
* The instance variables can only be accessed using a **getter** or a **setter** method with **public** access modifiers.
* Any place where a particular value can be used, a **method** call that returns *that type* can be used.

###Instance Variable Vs Local Variable.
* Instance variable always gets a default value. these default values are
|Data Type|Default Value|
|integers | 0 |
|floating points | 0.0|
|booleans | false|
|references | null|
* Instance variables are declared *inside a class* but not within a method.
* Local variables are declared *within a method*
* Local variables must be initialized before use

###Equality of primitive or reference
* Two *primitives* can be compared using the **==** operator.
* When **==** is used for equality check of references it just tells if both reference point to the same Heap Address.



Head First Java Chapter 05
=
This is the fifth Chapter learning of **Head First Java** by **Kathy Sierra** and **Bert Bates**, 
This markdown file is my notes for the fifth chapter, not sure if any copyright issues are there.

###Developing a Class.
* Figure out what the class is supposed to do.
* List the **instance variables and methods**.
* Write **prepcode** for the methods.
* Write **test code** for the methods.
* **Implement** the class.
* **Test** the methods.
* **Debug** and **reimplement** as needed

###for Loops.
####Regular (non-enhanced) for loops.
````java
for(int i =0; i < 100; i++)
````
#####Part One: initialization.
````java
int i =0;
````

#####Part two: boolean test.
````java
i < 100;
````
#####Part three: iteration expression
````java
i++;
````
####The enhanced for loop
````java
for(String name : nameArray){}
````
#####Part One: iteration variable declaration.
````java
String name
````

#####Part two: The Actual collection
````java
nameArray
````



Bullet Points
-
* Your java program should start with a high level design.
* Typically you'll write three things when you create a new class:
 * **prepcode**
 * **testcode**
 * **real(java) code.**
* Prepcode should descibe *what* to do, not *how* to do it. Implementation comes later.
* Use the prepcode to help design the test code.
* Write test code *before* you implement the methods.
* Choose *for* loops over *while* loops when you know how many times you want to repeat the loop code.
* Use the pre/post increment operator to add 1 to a variable (x++)
* Use the pre/post decrement operator to subtract 1 from a variable (x--).
* Use **Integer.parseInt()** to get the int value of a string.
* **Integer.parseInt()** works only if the String represents a digit ("0","1", etc).
* Use *break* to leave a loop early.



Head First Java Chapter 06
=
This is the sixth Chapter learning of **Head First Java** by **Kathy Sierra** and **Bert Bates**, 
This markdown file is my notes for the sixth chapter, not sure if any copyright issues are there.

### ArrayList
#### Something you can do with Arraylist.
##### Make one
````java
ArrayList<Egg> myList = new ArrayList<Egg>();
````
##### Put something in it.  
````java
Egg s = new Egg();  
myList.add(s);
```` 
##### Put another thing in it.  
````java
Egg b = new Egg();  
myList.add(b);
```` 
##### Find out how many things are in it.  
````java
int theSize = myList.size();
```` 
##### Find out if it contains something.  
````java
boolean isIn = myList.contain(s);
```` 
##### Find out where something is (i.e. its index)  
````java
boolean idx = myList.indexOf(b);  
```` 
##### Find out if it's empty
````java
boolean empty = myList.isEmpty();  
```` 
##### Remove something from it.  
````java
myList.remove(s);
````
#### ArrayList Vs Array.
* A plain old array has to know its size at the time it's created.
* To put an object in a regular array, you must assign it to a specific location.
* Arrays use array syntax that's not used anywhere else in java.
* ArrayList in Java 5.0 are parameterized.
#### Boolean Expressions.
Here are the Boolean Expression Used.
* **'And' and 'Or' Operators (&&, ||)**
* **Not equals (!= and !)**
* **Short Circuit Operators (&&, ||).**
 * In case of **&&** if the JVM sees that the left side of a && expression is false, it stops right there.
 * Similarly with **||**, the expression will be true if either side is true,
 
Bullet Points
-
* **ArrayList** is a class in the Java Api.
* To Put something into an ArrayList, use **add()**.
* To remove something from an ArrayList use **remove()**.
* To find out where something is in an ArrayList, use **indexOf()**.
* To find out if an ArrayList is empty, use **isEmpty()**.
* To get the size in an ArrayList, use the **size()** method.
* To get the **length** in a regular old array, you have to use the length variable.
* An ArrayList **resizes dynamically** to what-ever size is needed. It grows when objects are added, and it **shrinks** when objects are removed.
* You declare the type of the array using a **type parameter**, which is a type name in angle brackets.
* Although an ArrayList holds objects and not primitives, the compiler will automatically wrap a primitive into an object.
* Classes are grouped into packages.
* A class has a full name, which is a combination of the package name and the class name.
* To use class in a package other that java.lang, you must tell Java the full name of the class.
* You use either an import statement at the top of your source code, or you can type the full name every place you use the class in your code.



Head First Java Chapter 07
=
This is the seventh Chapter learning of **Head First Java** by **Kathy Sierra** and **Bert Bates**, 
This markdown file is my notes for the seventh chapter, not sure if any copyright issues are there.

BULLET POINTS
-
* A subclass extends a superclass.
* A subclass inherits all public instance variables and methods of the superclass, but does not inherit the private instance variables and methods of the superclass.
* Inherited methods can be overridden; instance variables cannot be overridden(although they can be redefined in the subclass).
* Use the IS-A test to verify that your inheritance hierarchy is valid.
* The IS-A relationship works in only one direction.
* When a method is overridden in a subclass, and that method is invoked on an instance of the subclass, the overridden version of the method is called.
* If a class extends A, and C extends B, class B IS-A class A, and class C IS-A class B, and Class C also IS-A class A.
* Instance variable and Class has a HAS-A relationship.

### Inheritance.
* Inheritance lets you guarantee that all classes grouped under a certain supertype have all the methods that the supertype has.
* When you define a supertype for a group of classes, any subclass of that supertype can be substituted where the supertype is expected.  

### Polymorphism.
* With polymorphism, the reference type can be a superclass of the actual object type.
* We can have polymorphic aguments and return type.(Write the method arguments as a superclass type, and you can pass any subclass object at the runtime.)

### Rules of overriding.
* Arguments must be the same, and return types must be compatible.
* The method can't be less accessible.

### Overloading.
* Method overloading is nothing more than having two methods with the same name and different argument list.
 * The return type can be different.
 * You can't change only the return type.
 * You can vary the access levels in any direction.



 Head First Java Chapter 08
=
This is the eighth Chapter learning of **Head First Java** by **Kathy Sierra** and **Bert Bates**, 
This markdown file is my notes for the eighth chapter, not sure if any copyright issues are there.

BULLET POINTS
-
* When you don't want a class to be instantiated mark the class with the **abstract** keywords.
* An abstract class can have both abstract and non-abstract methods.
* If a class has even one abstract method, the class must be marked abstract.
* An Abstract method has no body, and the declaration ends with a semi-colon.
* All abstract method must be implemented in the first concrete subclass in the inheritance tree.
* Every class in java is either a direct or indirect subclass of class **Object**.
* Methods can be declared with Object arguments and/or return types.
* You can call methods on an object only if the methods are in the class used as a reference variable type, regardless
of the actual object type.
* A reference variable of type Object can't be assigned to any other reference type without a cast, but at runtime
the cast will fail if the object on the heap is NOT a type compatible with the cast.
* All objects come out of the ArrayList<object> as type object.
* Multiple inheritance is not allowed in java because of the problems associated with the 'Deadly Diamond of Death'.
* An interface is like a 100% pure abstract class. It defines only abstract methods.
* Create an interface using the **interface** keyword instead of the word class.
* Implement an interface using the key word **implements**.
* Your class can implement multiple interfaces.
* A class that implements an interface must implement all the methods of the interface, since all **interface methods
are implicitly public and abstract**.
* To invoke the superclass version of a method from a subclass that'e overridden the method use the **super** keywords.



Head First Java Chapter 09
=
This is the nineth Chapter learning of **Head First Java** by **Kathy Sierra** and **Bert Bates**, 
This markdown file is my notes for the eighth chapter, not sure if any copyright issues are there.

BULLET POINTS
-
* Java has tow areas or memory we care about,
 1. The Stack
 2. The Heap
* Instance Variables are variables declared inside a class but outside any method.
* Local variables are variables declared inside a method or method parameters. 
* All local variables live on the stack, in the frame corresponding to the method where there variables are declared.
* Object reference variables work just like primitive variables - if the reference is declared as a local variables, it goes on the stack.
* All object live in the heap, regardless of whether the reference is a local or instance variable.
* Instance variables live within the object they belong to, on the heap.
* If the instance variables is a reference to an object, both the reference and the object it refers to are on the HEAP.
* A constructor is the code that runs when you say **new** on a class type.
* A constructor must have the same name as the class, and must *not* have a return type.
* You can use a constructor to initialize the state of the object being constructed.
* If you don't put constructor in your class, the compiler will put in a default constructor.
* The default constructor is always a no-args constructor.
* If you put a constructor-any constructor-in your class, the compiler will not build the default constructor.
* If you want a no-arg constructor, and you've already put in a constructor with arguments, you'll have to build the no-args constructor yourself.
* Always provide a no-args  if you can, to make it easy for programmers to make a working object, supply default values.
* Overloaded constructors means you have more than one constructor in your class.
* Overloaded constructors must have different argument lists.
* You cannot have two constructors with the same argument lists. An argument list includes the order and/or type of arguments.
* Instance variables are assigned a default value, even when you've not explicitly assign one.

### Constructors
* Constructors can be **public**, **private**,or **default**.
* Marking the Constructor as **private** doesn't mean nobody can access it, it just means that nobody outside the class can access it.
* All the constructors in an object's inheritance tree must run when you make a new object.
* Even Abstract class have constructors, Although you can never say new on an abstract class, an abstract class is still a super class, so its constructors runs when someone makes an instance of concrete subclass.
* The only way to call a super constructor is by calling **super()**, this calls the **super constructor**.
* Compiler puts a default call to **super()** if we don't. and it is always the no-args super which is inserted.
* The call to **super()** must be the first statement in each constructors.
* Use **this()** to call a constructor from another overloaded constructor in the same class.
* The Call to **this()** can be used only in a constructor, and must be the first statement in a constructor.
* A constructor can have a call to **super()** or **this()** but never both.

### Object Life and Scope
* An objects life depends on entirely on the life of references referring to it.
* A local variable lives only within the method that declared the variables.

````java
public void read(){
	int s = 42;
	// 's' can be used only within this method.
}
```` 

* An instance variable lives as long as the object does. If the object is still alive, so are its instance variables.

````java
public class life{
	int size;
	
	public setSize(int s){
	size = s;
	//'s' disappears at the end of the method,
	//but 'size' can be used anywhere in the class.
	}
}
````
* **life** A local variable is alive as long as its Stack frame is on the stack.
* **Scope** A local variable is in scope only within the method in which the variable was declared.

### Garbage Collection
* An object is alive as long as there are live references to it. If a reference variable goes out of scope but is still alive.
* Object are killed in these three ways
 1. Reference goes out of scope permanently.
 2. Assign the reference object to another object.
 3. Explicitly set the reference to null. 



 Head First Java Chapter 10
=
This is the tenth Chapter learning of **Head First Java** by **Kathy Sierra** and **Bert Bates**, 
This markdown file is my notes for the eighth chapter, not sure if any copyright issues are there.

BULLET POINTS
-
* A **static method** should be called using the class name rather than an object reference variable: **Math.random() vs myFoo.go()**.
* A static method can be invoked without any instances of the methods's class on the heap.
* A static method is good for a utility method that does not (and never will) depend on a particular instance variable value.
* A static method is not associated with a particular instance - only the class - so it cannot access any instance variable values of its class. It wouldn't know which instance's value to use.
* A static method cannot access a non-static method since non-static methods are usually associated with instance variable state.
* If you have a class with only static methods, and you do not want the class to be instantiated, you can mark the constructor private.
* A **static variable** is a variable shared by all members of a given class. There is only one copy of a static variable in a class, rather than one copy per each individual instance for instance variables.
* A static method can access a static variable.
* To make a constant in Java, mark a variable as both **static** and **final**.
* A final static variable must be assigned a value either at the time it is declared, or in a static initializer.

````java
static{
	DOG_CODE = 420;	
}
```` 
* The naming convention for constants is to make the name all uppercase.
* A final variable value cannot be changed once it has been assigned.
* Assigning a value to a *final* instance variable must be either at the time it is declared, or in the constructor.
* A final method cannot be overridden.
* A final class cannot be extended.

### Static Imports
* If you're going to use a static member a few times, we think you should avoid static imports, to help keep the code more readable.
* If you're going to use a static member a lot, then it is probably OK to use the static imports.
* Notice that you can use wildcards (*), in your static import declaration.
* A big issue with static imports is that it's not too hard to create naming conflicts.



Head First Java Chapter 11
=
This is the eleventh Chapter learning of **Head First Java** by **Kathy Sierra** and **Bert Bates**, 
This markdown file is my notes for the eleventh chapter, not sure if any copyright issues are there.

BULLET POINTS
-
* A method can throw an exception when something fails at runtime.
* An exception is always an object of type Exception.
* The compiler does NOT pay attention to exceptions that are of type **RuntimeException**. A RuntimeException does not have to be declared or wrapped in a try/catch.
* All Exceptions the compiler cares about are called **checked exceptions** which really means compiler-checked exceptions.
* A method throws an exception with the keywords **throw**, followed by a new exception object.

````java
throw new NoCaffeineException();

````

* Methods that might throw a checked exception must announce it with a throws Exception declarations.
* If your code calls a checked-exception-throwing method, it must reassure the compiler that precautions have been taken.
* If you're prepared to handle the exception, wrap the call in a try/catch, and put your exception handling/recovery code in the catch block.
* If you're not prepared to handle the exception, you can still make the compiler happy by officially 'ducking' the exception.

### Flow Control in try/catch block.
Take the example of the below code.

````java
try{
	Foo f = x.doRiskyThing();
	int b = f.getNum();
}catch (Exception e){
	System.out.println("Failed.");
}
System.out.println("We made it.");
````
If the try SUCCEEDS, the Catch block is not executed, and Last Sysout is printed.
If the Try fails, the rest of the try block never runs, and both the Sysout is printed.

### Finally
A finally block is where you put code that must run regardless of an exception.

````java
try{
	turnOvenOn();
	x.bake();
}catch (BakingException ex){
	ex.printStacktrace();
}finally{
	turnOvenOff();
}
````
A finally block lets you put all your import cleanup code in one place instead of duplicating it.
If the try or catch block has a return statement, finally will still run.

### Multiple Exception.
If a code throws multiple exceptions. 
* The catch block should be stacked one after the other. And the order of stacking is also important.
* Exceptions can be referred to polymorphically.
* You don't have to write a catch for each possible exception as long as the catch you have can handle any exception thrown.
 1. You can declare exceptions using a supertype of the exception you throw.
 2. You can CATCH exceptions using a super type of the exception thrown.
 3. Just because you CAN catch everything with one big super polymorphic catch, doesn't mean always you should.
* Multiple Catch block must be ordered from smallest to biggest.
* You can't put bigger baskets above smaller baskets.
* Siblings can be in any order, because they can't catch one another's exceptions.
* If you don't want to handle the exception in you code, declare the same exception in you code this is called DUCKING.

### Exception Rules
* You cannot have a catch or finally without a try.

The below code is not legal.
````java
	void go(){
		Foo f = new Foo();
		f.foof();
		catch (FooException ex){}
	}
````
* You cannot put code between the try and the catch.

The below code is not legal.
````java
try{
	x.doStuff();
}
int y = 43;
} catch (Exception ex){}
````
* A try MUST be followed by either a catch or finally.

The below code is legal.
````java
try{
	x.doStuff();
}finally{
	//CleanUp.
}
```` 

* A try with only a finally(no catch) must still declare the exception.

````java
void go() throws FooException{
	try{
		x.doStuff();
	}finally{}
}
````


Head First Java Chapter 14
=
This is the fourteenth Chapter learning of **Head First Java** by **Kathy Sierra** and **Bert Bates**, 
This markdown file is my notes for the fourteenth chapter, not sure if any copyright issues are there.

Serialization & File I/O
-

### Bullet Points (Serialization):-
* You can save an Object's state by serializing the Object.
* To serialize an object, you need an ObjectOutputStream.
* Streams are either connection streams or chain streams.
* Connections streams can represent a connection to a source or destination, typically file, network socket connection, or the console.
* Chain streams cannot connect to a source or destination and must be chained to a connection stream.
* To serialize an object, call *writeObject(theObject)* on the ObjectOutputStream. You do not need to call methods on the FileOutputStream.
* To be serialized, an object must implement the Serializable interface. If a superclass of the class implements Serializable, the subclass will automatically be serializable even if it does not specifically declare implements serializable.
* When an object is serialized, its entire object graph is serialized. That means any objects referenced by the serialized objects instance variable are serialized, and any object referenced by those object .. and so on.
* If any object in the graph is not serializable, an exception will be thrown at runtime, unless the instance variable referring to the object is skipped.
* Mark an instance variable with the *transient* keyword if you want serialization to skip that variable. The variable will be restored as null or default values.
* During deserialization, the class of all objects in the graph must be available to the JVM.
* You read object in (using readObject()) in the order in which they were originally written.
* The return type of readObject() is type Object, so deserialized objects must be cast to their real type.
* Static variables are not serialized! it doesn't make sense to save a static variable value as part of a specific object's state, since all objects of that type share only a single value - the one in the class.

### Bullet Points (File IO):-
* To write a text file, start with a FileWriter connection stream.
* Chain the FileWriter to a BufferedWriter for efficiency.
* A File object represent a file at a particular path, but does not represent the actual content of the file.
* With a File Object you can create, traverse, and delete directories.
* Most Streams that can use a String filename can use a File Object as well, and a File Object can be safer to use.
* To read a text file, start with a FileReader connection stream.
* Chain the FileReader to a BufferedReader for efficiency.
* To parse a text file, you need to be sure the file is written with some way to recognize the different elements. A common approach is to use some kind of character to separate the individual pieces.
* Use the String Split() method to split a String up into individual tokens. A String with one separator will have two tokens, one on each side of the separator. The *separator* doesn't count as a token.




Head First Java Chapter 15
=
This is the fifteenth Chapter learning of **Head First Java** by **Kathy Sierra** and **Bert Bates**, 
This markdown file is my notes for the fifteenth chapter, not sure if any copyright issues are there.

Networking & Threads
-

### Bullet Points (Networking):-
* Client and server applications communicate over a Socket connections.
* A Socket represents a connection between two applications which may (or may not) be running on two different physical machines.
* A client must know the IP Address(or domain name) and TCP port number of the server application.
* A TCP port is a 16-bit unsigned number assigned to a specific server application. TCP port numbers allow different clients to connect to the same machine but communicate with different applications running on that machine.
* The port number from 0 to 1023 are reserved for 'well known services' including HTTP, FTP, SMTP, etc.
* A client connects to a server by making a Server socket

````java
Socket s = new Socket("127.0.0.1",4242);
````

* Once connected, a client can get input and output streams from the socket. These are low-level 'connection' streams.

````java
sock.getInputStream()
````

* To read text data from the server, create a BufferedReader, chained to an InputStreamReader, which is chained to the input stream from the Socket.
* InputStreamReader is a 'bridge' stream that takes in bytes and converts them to text (character) data. It's used primarily to act as the middle chain between the high-level BufferedReader and the low-level socket input stream.
* To write text data to the server, create a PrintWriter chained directly to the Socket's output stream. Call the print() or println() methods to send Strings to the server.
* Servers use a ServerSocket that waits for client requests on a particular port number.
* When a ServerSocket gets a request, it 'accepts' the request by making a Socket Connection with the client.

### Bullet Points (Threads):-
* A thread with a lower-case 't' is a separate thread of execution in Java.
* Every thread in Java has its own call stack.
* A Thread with a capital 'T' is the java.lang.Thread class. A Thread object represents a thread of execution.
* A Thread needs a job to do. A Thread's job is an instance of something that implements the Runnable interface.
* The Runnable interface has just a single method, run(), This is the method that goes on the bottom of the new call stack. In other words, it is the first method to run in the new thread.
* To launch a new thread, you need a Runnable to pass to the Thread's constructor.
* A thread is in the NEW state when you have instantiated a Thread object but have not yet called start().
* When you start a thread , a new stack is created, with the Runnable's run() method on the bottom of the stack.The thread is now in the RUNNABLE state, waiting to be chosen to run.
* A thread is said to be RUNNING when the JVMs thread scheduler has selected it to be the currently-running thread. On a single processor machine, there can be only one currently running thread.
* Sometimes a thread can be moved from the RUNNING state to a BLOCKED state. A thread might be blocked because it's waiting for data from a stream, or because it has gone to sleep, or because it is waiting for an object's lock.
* Thread scheduling is not guaranteed to work in any particular way, so you cannot be certain that threads will take turns nicely, You can help influence turn-taking by putting your threads to sleep periodically.

### Bullet Points (Threads Sleep):-
* The static Thread.sleep() method forces a thread to leave the running state for at least the duration passed to the sleep method.
* The sleep() method throws a checked exception (InterruptedException) so all calls to sleep() must be wrapped in a try/catch, or declared.
* You can sleep() to help make sure all threads get a chance to run, although there's no guarantee that when a thread wakes up it'll go to the end of the runnable line. It might, for example, go right back to the front.
* You can name a thread using the setName() method. All threads get a default name, but giving them a explicit name can help you keep tracks of threads, especially if you're debugging with print statements.
* You can have serious problems with threads if two or more threads have access to the same object on the heap.
* Two or more threads accessing the same object can lead to data corruption if one thread, for example, leaves the running state while still in the middle of manipulating an object's critical state.
* To make your objects thread-safe, decide which statements should be treated as one atomic process.
* Use the keywords **synchronized** to modify a method declaration, when you want to prevent two threads from entering that method.
* Every object has a single lock, with a single key for that lock. Most of the time we don't care about that lock; lock come into play only when an object has synchronized methods.
* When a thread attempts to enter a synchronized method, the thread must get the key for the object. If the key is not available, the thread goes into a kind of waiting lounge, until the key becomes available.
* Even if an object has more than one synchronized method, there is still only one key. Once any thread has entered a synchronized method on that object, no thread can enter any other synchronized method on the same object. This restriction lets you protect your data by synchronizing any method that manipulates the data.




Head First Java Chapter 16
=
This is the Sixteenth Chapter learning of **Head First Java** by **Kathy Sierra** and **Bert Bates**, 
This markdown file is my notes for the Sixteenth chapter, not sure if any copyright issues are there.

Collections with Generics
-

### ArrayList
* ArrayList does not have a sort method.
* ArrayList is not the only Collection
  * **TreeSet** : Keeps the elements sorted and prevents duplicates.
  * **HashMap** : Store and Access elements as name/value pairs.
  * **LinkedList** : Gives better performance when you insert or delete elements from middle.
  * **HashSet** : Prevents duplicates in the collection, and given an element, can find that element quickly.
  * **LinkedHashMap** : It remembers the order in which elements were inserted in addition to HashMap.
* To get the sort functionality from ArrayList we can change it to a TreeSet
  * **BUT** TreeSet might be more expensive. Every insert into a TreeSet requires hugh time to figure out where it should reside.

### sort()
````java
	static <T extends Comparable<? super T>> void 	sort(List<T> list)
````
* Sorts the specified list into ascending order, according to the natural ordering of its elements.
* The sort method declaration looks little strange. Because the Collection framework make heavy use of *generics*.

### Generics
* Generics means more type-safety.
* With generics, you can create type-safe collections where more problems are caught at compile-time instead of runtime.
* Without generics, the compiler would happily let you put a Pumpkin into an ArrayList that was supposed to hold only Cat Objects.
* Three things are of importance while dealing with generics.
  * Create instances of generified classes (like ArrayList)
  ````java
  	new ArrayList<Song>();
  ````
  * Declaring and assigning variables of generic types.
  ````java
  	List<Song> songList = new ArrayList<Song>();
  ````
  * Declaring (and invoking) methods that take generic types.
  ````java
  	void foo(List<Song> list);
  	x.foo(songList);
  ````
  
### Generic Classes
````java
	public class ArrayList<E>
	extends AbstractList<E>
	implements List<E>, RandomAccess, Cloneable, Serializable  
````
* Think of 'E' as a stand-in for "the type of element you want this collection to hold and return."

### Generic Methods.
* A generic method means that the method declaration uses a type parameter in its signature. It is used in this manner.
  * Using the type parameter defined in the class declaration.
  ````java
  	public class ArrayList<E> extends AbstractList<E>{
  		public boolean add(E o);
  	}
  ````
  * Using a type parameter that was NOT defined in the class definition.
  ````java
  	public <T extends Animal> void takeThing(ArrayList<T> list);
  	
  ````
* Difference between the below Code sample.
````java
	public <T extends Animal> void takeThing(ArrayList<T> list);
````
  * This one where **<T extends Animal>** is part of the method declaration, means that any ArrayList declared of a type that is Animal, or one of Animal's sub type is legal.  
**AND**
````java
	public void takeThing(ArrayList<Animal> list);
````
  * This method argument means that only an **ArrayList<Animal>** is legal and not sub type.
    * If you declare a method to take ArrayList<Animal> it can only take an ArrayList<Animal>, not ArrayList<Dog>.
    * Array types are checked again at runtime, but collection type checks happens only when you compile.
### Genrics Implement and Extends
* In generics, the keywords "extends" really means "is-a" and works for BOTH classes and interfaces.

### Collection API.
* There are three main interfaces, **List**,**Set**, and **Map**.
  1. **LIST** : **Where sequence matters.**
  2. **SET** : **Where uniqueness matters.**
  3. **MAP** : **Where finding something by key matters.**
    1. Map interface doesn't actually extend the Collection interface.
#### Object Equality
* There are two type of Equality.
  1. Reference Equality
    * Two reference, one object on the heap.
    * If you call **hashCode()** method on both reference, you'll get same result.
  2. Object Equality.
    * Two reference, two objects on the heap, but the objects are considered meaningfully equivalent.
    * We must override the **hashCode()** and **equals()** methods.

### HashSet
* A HashSet checks the hasCodes, if they are different the object are assumed to be different.

### TreeSet 
* A TreeSet is similar to HashSet in that it prevents duplicates, and it also keeps the list sorted.
* To use a TreeSet, one of these things must be true.
  * The element in the list must be of a type that implements **Comparable**.  
    **OR**  
  * You use the TreeSet's overloaded constructor that takes a Comparator.    

### Map
* Each element in a Map is actually TWO Objects - a *key* and a *value*. You can have duplicate values, but NOT Duplicate keys.    

### Generic WildCards
* There is a way a method argument that can accept an ArrayList of any Animal sub type.

````java
public void takeAnimal(ArrayList <? extends Animal> animals){
	for (Animal animal : animals) {
			animal.eat();
		}
}
````
**OR**

````java
public <T extends Animal>void takeAnimal(ArrayList <T> animals){
	for (Animal animal : animals) {
			animal.eat();
		}
}
````
* When you use a wild card in you method argument, the compiler will STOP you from doing anything that could hurt the list referenced by the method parameters.
* You can still invoke methods on the elements in the list, but you cannot add elements to the list.
* In other words, you can do things with the list elements, but you cannot put new things in the list.
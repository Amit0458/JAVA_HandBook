# JAVA_HandBook

## Java Platform 

**Why is Java so Popular?**

```
Java is an object-oriented computer language. 
The code is particularly robust since Java objects do not have any references to data outside 
of themselves. 
We utilize Java to create full-fledged web applications. 
Execute web applications on a single computer or across a network of servers and clients.

Two main reasons for popularity of Java are
 • 1. Platform Independence
 • 2. Object Oriented Language

```

**What is Platform Independence?**

```
 Software that can run on a variety of hardware platforms or software architectures. 
 Platform-independent software can be used in many different environments, requiring less planning
 and translation across an enterprise.
 
 Java programming language was designed to run on multiple types of hardware and multiple 
 operating systems. If Java platform-independence becomes a reality, organizations with multiple 
 types of computers will be able to write a specialized application once and have it be used by 
 virtually everyone, rather than having to write, distribute and maintain multiple versions of the 
 same program.
 
```

**What is ByteCode?**

```
Bytecode is computer object code that an interpreter converts into binary machine code so it can be read 
by a computer's hardware processor.

```

**Compare JDK vs JVM VS JRE.**

```
1. JVM 
	a. Virtual machine that run the Java bytecode.
	b. Makes java portable.

2. JRE
  a. JVM + Libraries + Other Components. 
	   to run applets and other java applications

3. JDK
	a. JRE + Compilers + Debuggers

```

**What is the role of class loader in java ?**

```
The Java ClassLoader is a part of the Java Runtime Environment that dynamically loads Java classes 
into the Java Virtual Machine. The Java run time system does not need to know about files and file 
systems because of classloaders. Java classes aren’t loaded into memory all at once, but when required 
by an application. At this point, the Java ClassLoader is called by the JRE and these ClassLoaders 
load classes into memory dynamically.

```

## Wrapper Classes

**What are wrapper classes? **
```
The wrapper class in Java provides the mechanism to convert primitive into object and object into primitive.
All of the primitive wrapper classes in Java are immutable.

Wrapper   : Boolean, Byte, Character, Double, Float, Integer, Long, Short
Primitive : boolean, byte, char ,double, float, int , long, short

```

**Why do we need Wrapper Classes in Java?**

```
A wrapper class wraps (encloses) around a data type and gives it an object appearance.

Reasons why we need Wrapper Classes
	• null is a possible value
	• use it in a Collection 
	• Methods that support Object like creation from other types.. like String 
	Integer number2 = new Integer("55");//String

```

**What are the different ways of creating Wrapper Class Instances?**

```
Integer number = new Integer(76);//int
Integer number2 = new Integer("96");//String

Float number3 = new Float(45.0);//double argument
Float number4 = new Float(55.0f);//float argument
Float number5 = new Float("55.0f");//String

Character c1 = new Character('C');//Only char constructor
//Character c2 = new Character(124);//COMPILER ERROR

Boolean b = new Boolean(true);
//"true" "True" "tRUe" - all String Values give True
//Anything else gives false
Boolean b1 = new Boolean("true");//value stored - true
Boolean b2 = new Boolean("True");//value stored - true
Boolean b3 = new Boolean("False");//value stored - false
Boolean b4 = new Boolean("SomeString");//value stored - false

valueOf Static Methods
Provide another way of creating a Wrapper Object

Integer hundred = Integer.valueOf("100");//100 is stored in variable
Integer seven = Integer.valueOf("111", 2);//binary 111 is converted to 

```

**What is Auto Boxing?**

```
Autoboxing is the automatic conversion that the Java compiler makes between the primitive types and 
their corresponding object wrapper classes. For example, converting an int to an Integer, 
a double to a Double, and so on.

Character ch = 'a';

List<Integer> li = new ArrayList<>();
for (int i = 1; i < 50; i += 2)
    li.add(i);

```

** What are the advantages of Auto Boxing?**

```
No need of conversion between primitives and Wrappers manually so less coding is required.

-Auto Boxing uses the static valueOf methods.

-Less code to writing.
-The code looks cleaner.
-The best strategy for transformation is consequently picked, e.g. Integer.valueOf (int) is utilized rather than new Integer (int)

Integer nineC = 9;
Integer nineD = 9;
System.out.println(nineC == nineD);//true
System.out.println(nineC.equals(nineD));//true

```

**What is Casting?**

```
Casting is used when we want to convert one data type to another.

There are two types of Casting
• Implicit Casting
• Explicit Casting

```

**What is Implicit Casting?**

```
-Implicit Casting is done by the compiler.

In implicit typecasting, the conversion involves a smaller data type to the larger type size. For example, the byte datatype implicitly typecast into short, char, int, long, float, and double. The process of converting the lower data type to that of a higher data type is referred to as Widening.

int value = 100;
long number = value; //Implicit Casting
float f = 100; //Implicit Casting

```

**What is Explicit Casting?**

```
Explicit Casting is done with the help of cast operator.

	double a = 100.245;
      
      Narrowing Type Casting
    	short b = (short) a;
    	int c = (int) a;

Explicit casting would cause truncation of value if the value stored is greater 
than the size of the variable.
	int bigValue = 280;
	byte small = (byte) bigValue;
	System.out.println(small);//output 24. Only 8 bits remain.


```

## Strings 

**Are all String’s immutable?**

```

```

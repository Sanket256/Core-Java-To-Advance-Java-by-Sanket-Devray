# Core-Java-To-Advance-Java-by-Sanket-Devray


Basic Java
Introduction to Java ->
1) History and Features of Java:

1)History: Java was developed by Sun Microsystems (now owned by Oracle) and released in 1995. It was designed to have the "write once, run anywhere" capability.
2)Features: Object-oriented, platform-independent, simple, secure, robust, portable, multithreaded, high performance, and distributed.
3)Setting up the Java Development Kit (JDK):

The JDK includes tools for developing and testing Java programs. You can download it from Oracle's official website or other sources like OpenJDK.
Java Runtime Environment (JRE) and Java Virtual Machine (JVM):

JRE: Provides the libraries, Java Virtual Machine (JVM), and other components to run applications written in Java.
JVM: An engine that provides a runtime environment to execute Java bytecode. It is platform-dependent.

2) Basic Syntax :
Structure of a Java Program (Classes, Methods):

Every Java program has at least one class and a main method. The class name must match the file name.
Example:

public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}

Writing and Running Your First Java Program (Hello World):

-Save the code in a file named HelloWorld.java.
-Compile the program using javac HelloWorld.java.
-Run the compiled bytecode using java HelloWorld.
-Data Types and Variables

3) Primitive Data Types:

1)byte: 1 byte

Description: An 8-bit signed integer.
Range: -128 to 127.
Use Case: Useful for saving memory in large arrays, where the memory savings actually matters.
Example:

        byte age = 25;
        System.out.println("Age: " + age); 
        // Output: Age: 25
        
2)short: 2 bytes
 
Description: A 16-bit signed integer.
Range: -32,768 to 32,767.
Use Case: Can be used to save memory as compared to int when you know the value will be within this range.
Example:

        short year = 2024;
        System.out.println("Year: " + year);
        // Output: Year: 2024
        
3)int: 4 bytes

Description: A 32-bit signed integer.
Range: -2^31 to 2^31 - 1 (-2,147,483,648 to 2,147,483,647).
Use Case: The default choice for integral values unless there's a reason to use a smaller or larger type.
Example:

        int population = 1500000;
        System.out.println("Population: " + population); 
        // Output: Population: 1500000
        
4)long: 8 bytes

Description: A 64-bit signed integer.
Range: -2^63 to 2^63 - 1 (-9,223,372,036,854,775,808 to 9,223,372,036,854,775,807).
Use Case: Used when a wider range than int is needed.
Example:

        long distance = 123456789L; // Note the 'L' suffix to denote a long literal
        System.out.println("Distance: " + distance); 
        // Output: Distance: 123456789
        
5)float: 4 bytes

Description: A single-precision 32-bit IEEE 754 floating point.
Range: Approximately ±3.40282347E+38F (6-7 significant decimal digits).
Use Case: Useful for saving memory in large arrays of floating point numbers.
Example:

        float price = 19.99f; // Note the 'f' suffix to denote a float literal
        System.out.println("Price: " + price); 
        // Output: Price: 19.99
        
6)double: 8 bytes

Description: A double-precision 64-bit IEEE 754 floating point.
Range: Approximately ±1.79769313486231570E+308 (15 significant decimal digits).
Use Case: The default choice for decimal values.
Example:

        double pi = 3.141592653589793;
        System.out.println("Pi: " + pi); 
        // Output: Pi: 3.141592653589793
        
7)char: 2 bytes

Description: A single 16-bit Unicode character.
Range: 0 to 65,535 (unsigned).
Use Case: Used to store any character.
Example:

        char initial = 'A';
        System.out.println("Initial: " + initial); 
        // Output: Initial: A
        
8)boolean: 1 bit info (0 or 1) 

Description: Represents one bit of information, but its "size" isn't precisely defined.
Values: Only two possible values: true and false.
Use Case: Used for simple flags that track true/false conditions.
Example:

        boolean isJavaFun = true;
        System.out.println("Is Java fun? " + isJavaFun); 
        // Output: Is Java fun? true
Summary Table

Type	Size	Range	                                                   Example
byte	8-bit	-128 to 127	                                           byte age = 25;
short	16-bit	-32,768 to 32,767	                                 short year = 2024;
int	    32-bit	-2^31 to 2^31 - 1	                                int population = 1500000;
long	64-bit	-2^63 to 2^63 - 1	                                long distance = 123456789L;
float	32-bit	±3.40282347E+38F (6-7 significant decimal digits)	float price = 19.99f;
double	64-bit	±1.79769313486231570E+308 (15 significant digits)	double pi = 3.141592653589793;
char	16-bit	0 to 65,535 (unsigned)	                            char initial = 'A';
boolean	1-bit	true or false	                                     boolean isJavaFun = true;


4) Non-Primitive Data Types:

1) Strings: A String is a sequence of characters. In Java, strings are objects that represent sequences of characters.
Example:

        String message = "Hello, World!";
        System.out.println(message);
        // Output: Hello, World!
   
2)Arrays: An array is a container object that holds a fixed number of values of a single type. The length of an array is established when the array is created.
Example:

            int[] numbers = {1, 2, 3, 4, 5};
            System.out.println(numbers[0]); // Output: 1
            System.out.println(numbers[4]); // Output: 5

3) Classes: A class is a blueprint for creating objects. A class defines a datatype by bundling data and methods that work on the data into one single unit.
Example:

        public class Person {
            String name;
            int age;
        
            // Constructor
            public Person(String name, int age) {
                this.name = name;
                this.age = age;
            }
        
            // Method to display person details
            public void display() {
                System.out.println("Name: " + name + ", Age: " + age);
            }
        
            public static void main(String[] args) {
                Person person = new Person("Alice", 30);
                person.display(); // Output: Name: Alice, Age: 30
            }
        }

5) Variables: Declaring and Initializing Variables:

            Declaring: int number;
            Initializing: number = 10;
            Combined: int number = 10;

            Constants Using final:
            final int MAX_VALUE = 100; // MAX_VALUE cannot be changed.

6) Operators
   Arithmetic Operators: +, -, *, /, %

        int sum = 5 + 3; // 8

   Relational Operators: ==, !=, >, <, >=, <=
   
        boolean isEqual = (5 == 3); // false

   Logical Operators: &&, ||, !

        boolean result = (5 > 3) && (3 < 4); // true

   Bitwise Operators: &, |, ^, ~, <<, >>, >>>

        int bitwiseAnd = 5 & 3; // 1

   Assignment Operators: =, +=, -=, *=, /=, %=

        int a = 5;
        a += 3; // a is now 8
   
   Unary Operators: +, -, ++, --, !

        int b = 5;
        b++; // b is now 6

   Ternary Operator: ? :
   
        int min = (a < b) ? a : b;

7) ontrol Flow Statements:

1)Decision Making:

if:

        if (a > b) {
            System.out.println("a is greater than b");
        }
        
if-else:

        if (a > b) {
            System.out.println("a is greater than b");
        } else {
            System.out.println("a is not greater than b");
        }

switch:

        int day = 2;
        switch (day) {
            case 1:
                System.out.println("Monday");
                break;
            case 2:
                System.out.println("Tuesday");
                break;
            default:
                System.out.println("Other day");
        }
        
2)Looping:

for:

        for (int i = 0; i < 5; i++) {
            System.out.println(i);
        }
        
while:

        int j = 0;
        while (j < 5) {
            System.out.println(j);
            j++;
        }
        
do-while:

        int k = 0;
        do {
            System.out.println(k);
            k++;
        } while (k < 5);

3) Branching:

break: Exits the loop or switch statement.

        for (int i = 0; i < 5; i++) {
            if (i == 3) break;
            System.out.println(i);
        }
        
continue: Skips the current iteration of the loop.

        for (int i = 0; i < 5; i++) {
            if (i == 3) continue;
            System.out.println(i);
        }
        
return: Exits from the current method and optionally returns a value.

        public int add(int a, int b) {
            return a + b;
        }

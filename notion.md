# JAVA Full Notes

<aside>
🔖 ***Table of Contents:***

***Basics***

- [**File, Code, Compile**](https://www.notion.so/File-Code-Compile-b1cfda2879814e6b90c1b8ddcfeee0e6?pvs=21)
- [**Boilerplate**](https://www.notion.so/Boilerplate-70325c6b17de4097aeceddd12c39a9b7?pvs=21)
- [**Output**](https://www.notion.so/Output-40ca369ef57d4991be0475ec1933893e?pvs=21)
- [**Inputs**](https://www.notion.so/Inputs-6072adcbd26b4e838f9d81f05cfac4cd?pvs=21)
- [**Comments**](https://www.notion.so/Comments-ba454e06037c4fbdbe61d453245ca43d?pvs=21)
- [**Concatination**](https://www.notion.so/Concatination-10c38bb8d2224a179e1221bebc721c32?pvs=21)
- [**Rules**](https://www.notion.so/Rules-c2e3af25e76d442991fda8be0a132604?pvs=21)

***Variables & Datatypes***

- [**Variables**](https://www.notion.so/Variables-a90af54560a347ea9537d3d13c8cfa08?pvs=21)
- [**Types of Variables**](https://www.notion.so/Types-of-Variables-4553934e93e64f43a7589c1b75629dbf?pvs=21)
    
    (Instance, Local, Static)
    
- [**Data Types**](https://www.notion.so/Data-Types-243edbb9197b47dbbf05d21ce823d777?pvs=21)
    - [***Primitive Data Types:***](https://www.notion.so/Primitive-Data-Types-47de61b0ba894e32932256e1f7a05b04?pvs=21)
        
        (`int`, `byte`, `float`, `boolean`. etc.)
        
    - [***Non-primitive Data Types:***](https://www.notion.so/Non-primitive-Data-Types-a56538151c47447d99a721af20ebbec6?pvs=21)
        
        (`String`, `Array`, `Class`, etc.)
        
- 

***Type Operations***

**Type Conversion**

**Type Casting**

***OOPs***

***Data Structures***

1. Array
2. String

***Algorithms***

</aside>

<aside>
💡 **File, Code, Compile**

</aside>

- `***.java` File Creation:***
    - *Step-1:* Create a `.java` file.
    - *Step-2:* Code must start with a `public class`, and that **class name** (if `public class JavaBasics`) should be **same** with **file name** (`*JavaBasics.java*`)
    - *Step-3:* Then call **main** function
- ***Structure:*** `**Class -> Codes and Functions**`
- ***Statement Terminator → `;`***
- ***Compile & Run:***
    
    ```bash
    $ javac JavaNew.java
    $ java JavaNew.java
    ```
    
    - In Terminal, first navigate to open folder where `*.java*` file is present
    - Then use `javac FileName.java` to compile `*.java*` file → it creates `*.class*` file with same name
    - A `*.class*` file is compiled form of a `*.java*` file → contains Java bytecode that can be executed by JVM
    - Then use `java FileName.java` → to run

<aside>
💡 **Boilerplate**

</aside>

```java
public class JavaBasics {
    public static void main(String args[]) {
			...
    }
}
```

- `public static` → is Access Modifier (check OOPs).
- `void` → is a return type which returns nothing.
- `void main()` → `returnType functionName()` (check Function Syntax).
- `main()` → is a inbuilt Function, so we **can’t use main keyword anywhere else** in Java code.
- Here main function taking a string as input, that is an array named `args[]` (or arguments).
- So, `void` is **output** and `String args[]` is **input** of `main` function.

<aside>
💡 **Output**

</aside>

- `System.out.print(“Hello Java”);` -> Full statement use to print *“Hello Java”* in Terminal.

[data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEgAAABICAYAAABV7bNHAAAA1ElEQVR4Ae3bMQ4BURSFYY2xBuwQ7BIkTGxFRj9Oo9RdkXn5TvL3L19u+2ZmZmZmZhVbpH26pFcaJ9IrndMudb/CWadHGiden1bll9MIzqd79SUd0thY20qga4NA50qgoUGgoRJo/NL/V/N+QIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIEyFeEZyXQpUGgUyXQrkGgTSVQl/qGcG5pnkq3Sn0jOMv0k3Vpm05pmNjfsGPalFyOmZmZmdkbSS9cKbtzhxMAAAAASUVORK5CYII=](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEgAAABICAYAAABV7bNHAAAA1ElEQVR4Ae3bMQ4BURSFYY2xBuwQ7BIkTGxFRj9Oo9RdkXn5TvL3L19u+2ZmZmZmZhVbpH26pFcaJ9IrndMudb/CWadHGiden1bll9MIzqd79SUd0thY20qga4NA50qgoUGgoRJo/NL/V/N+QIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIEyFeEZyXQpUGgUyXQrkGgTSVQl/qGcG5pnkq3Sn0jOMv0k3Vpm05pmNjfsGPalFyOmZmZmdkbSS9cKbtzhxMAAAAASUVORK5CYII=)

- `print()` -> `print` function to print only output.
    
    [data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEgAAABICAYAAABV7bNHAAAA1ElEQVR4Ae3bMQ4BURSFYY2xBuwQ7BIkTGxFRj9Oo9RdkXn5TvL3L19u+2ZmZmZmZhVbpH26pFcaJ9IrndMudb/CWadHGiden1bll9MIzqd79SUd0thY20qga4NA50qgoUGgoRJo/NL/V/N+QIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIEyFeEZyXQpUGgUyXQrkGgTSVQl/qGcG5pnkq3Sn0jOMv0k3Vpm05pmNjfsGPalFyOmZmZmdkbSS9cKbtzhxMAAAAASUVORK5CYII=](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEgAAABICAYAAABV7bNHAAAA1ElEQVR4Ae3bMQ4BURSFYY2xBuwQ7BIkTGxFRj9Oo9RdkXn5TvL3L19u+2ZmZmZmZhVbpH26pFcaJ9IrndMudb/CWadHGiden1bll9MIzqd79SUd0thY20qga4NA50qgoUGgoRJo/NL/V/N+QIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIEyFeEZyXQpUGgUyXQrkGgTSVQl/qGcG5pnkq3Sn0jOMv0k3Vpm05pmNjfsGPalFyOmZmZmdkbSS9cKbtzhxMAAAAASUVORK5CYII=)
    
- `println()` -> `println` function to print a output and create next line.
    
    [data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEgAAABICAYAAABV7bNHAAAA1ElEQVR4Ae3bMQ4BURSFYY2xBuwQ7BIkTGxFRj9Oo9RdkXn5TvL3L19u+2ZmZmZmZhVbpH26pFcaJ9IrndMudb/CWadHGiden1bll9MIzqd79SUd0thY20qga4NA50qgoUGgoRJo/NL/V/N+QIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIEyFeEZyXQpUGgUyXQrkGgTSVQl/qGcG5pnkq3Sn0jOMv0k3Vpm05pmNjfsGPalFyOmZmZmdkbSS9cKbtzhxMAAAAASUVORK5CYII=](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEgAAABICAYAAABV7bNHAAAA1ElEQVR4Ae3bMQ4BURSFYY2xBuwQ7BIkTGxFRj9Oo9RdkXn5TvL3L19u+2ZmZmZmZhVbpH26pFcaJ9IrndMudb/CWadHGiden1bll9MIzqd79SUd0thY20qga4NA50qgoUGgoRJo/NL/V/N+QIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIEyFeEZyXQpUGgUyXQrkGgTSVQl/qGcG5pnkq3Sn0jOMv0k3Vpm05pmNjfsGPalFyOmZmZmdkbSS9cKbtzhxMAAAAASUVORK5CYII=)
    
- `(“....\n....\n”)` -> `\n` creates line break or new line in output argument.
- *Example:*
    
    ```java
    public class JavaNew {
        public static void main(String args[]) {
            System.out.println("Hello Java \nI love Java");
    				/*OP: Hello Java 
    							I love Java*/
        }
    }
    ```
    

<aside>
💡 **Inputs**

</aside>

- `Scanner` class is used to take inputs in Java.
- Fist we need to import `util` package for using `Scanner` class by
    
    `import java.util.*;` → `*` means we are importing everything of that package
    
- Then we need to create a new object `sc` of scanner class →
    
    `Scanner sc = new Scanner(System.in);`
    
- Like `System.out` in Output → Here we need to write `System.in`
- Then `next()` function helps, `sc` object to catch input given by User →
    
    `String name = sc.next();`
    
- `next()` function has many variants ->
    - **`next()`** → Captures until a space.
    - `**nextLine()**` → Captures a whole String with spaces also.
    - `**nextInt()**` → Captures Integers.
    - **`nextFloat()` →** Captures Float.
    - **`nextDouble()` →** Captures Double.
    - **`nextBoolean()` →** Captures Boolean.
    - **`nextShort()` →** Captures Short.
    - **`nextLong()` →** Captures Long.
    
    [data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEgAAABICAYAAABV7bNHAAAA1ElEQVR4Ae3bMQ4BURSFYY2xBuwQ7BIkTGxFRj9Oo9RdkXn5TvL3L19u+2ZmZmZmZhVbpH26pFcaJ9IrndMudb/CWadHGiden1bll9MIzqd79SUd0thY20qga4NA50qgoUGgoRJo/NL/V/N+QIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIEyFeEZyXQpUGgUyXQrkGgTSVQl/qGcG5pnkq3Sn0jOMv0k3Vpm05pmNjfsGPalFyOmZmZmdkbSS9cKbtzhxMAAAAASUVORK5CYII=](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEgAAABICAYAAABV7bNHAAAA1ElEQVR4Ae3bMQ4BURSFYY2xBuwQ7BIkTGxFRj9Oo9RdkXn5TvL3L19u+2ZmZmZmZhVbpH26pFcaJ9IrndMudb/CWadHGiden1bll9MIzqd79SUd0thY20qga4NA50qgoUGgoRJo/NL/V/N+QIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIEyFeEZyXQpUGgUyXQrkGgTSVQl/qGcG5pnkq3Sn0jOMv0k3Vpm05pmNjfsGPalFyOmZmZmdkbSS9cKbtzhxMAAAAASUVORK5CYII=)
    
    [data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEgAAABICAYAAABV7bNHAAAA1ElEQVR4Ae3bMQ4BURSFYY2xBuwQ7BIkTGxFRj9Oo9RdkXn5TvL3L19u+2ZmZmZmZhVbpH26pFcaJ9IrndMudb/CWadHGiden1bll9MIzqd79SUd0thY20qga4NA50qgoUGgoRJo/NL/V/N+QIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIEyFeEZyXQpUGgUyXQrkGgTSVQl/qGcG5pnkq3Sn0jOMv0k3Vpm05pmNjfsGPalFyOmZmZmdkbSS9cKbtzhxMAAAAASUVORK5CYII=](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEgAAABICAYAAABV7bNHAAAA1ElEQVR4Ae3bMQ4BURSFYY2xBuwQ7BIkTGxFRj9Oo9RdkXn5TvL3L19u+2ZmZmZmZhVbpH26pFcaJ9IrndMudb/CWadHGiden1bll9MIzqd79SUd0thY20qga4NA50qgoUGgoRJo/NL/V/N+QIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIEyFeEZyXQpUGgUyXQrkGgTSVQl/qGcG5pnkq3Sn0jOMv0k3Vpm05pmNjfsGPalFyOmZmZmdkbSS9cKbtzhxMAAAAASUVORK5CYII=)
    
    [data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEgAAABICAYAAABV7bNHAAAA1ElEQVR4Ae3bMQ4BURSFYY2xBuwQ7BIkTGxFRj9Oo9RdkXn5TvL3L19u+2ZmZmZmZhVbpH26pFcaJ9IrndMudb/CWadHGiden1bll9MIzqd79SUd0thY20qga4NA50qgoUGgoRJo/NL/V/N+QIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIEyFeEZyXQpUGgUyXQrkGgTSVQl/qGcG5pnkq3Sn0jOMv0k3Vpm05pmNjfsGPalFyOmZmZmdkbSS9cKbtzhxMAAAAASUVORK5CYII=](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEgAAABICAYAAABV7bNHAAAA1ElEQVR4Ae3bMQ4BURSFYY2xBuwQ7BIkTGxFRj9Oo9RdkXn5TvL3L19u+2ZmZmZmZhVbpH26pFcaJ9IrndMudb/CWadHGiden1bll9MIzqd79SUd0thY20qga4NA50qgoUGgoRJo/NL/V/N+QIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIECBAgQIAAAQIEyFeEZyXQpUGgUyXQrkGgTSVQl/qGcG5pnkq3Sn0jOMv0k3Vpm05pmNjfsGPalFyOmZmZmdkbSS9cKbtzhxMAAAAASUVORK5CYII=)
    
- *Example:*
    
    ```java
    import java.util.*;
    
    public class JavaNew {
        public static void main(String args[]) {
            Scanner sc = new Scanner(System.in);
            String a = sc.next();
            System.out.println(a);
        }
    }
    ```
    

<aside>
💡 **Comments**

</aside>

- Single line comment out → `//`
- Multi line comment out → `/* … */`

<aside>
💡 **Concatination**

</aside>

- We can use `+` operator to combine multiple Strings →

```java
String firstName = "John";
String lastName = "Doe";
System.out.println(firstName + " " + lastName);
```

- We can also use `concat()` method for concatination
- Or, for loop concatination `StringBuilder` or `StringBuffer`’s `appned()` method is usable

<aside>
💡 **Variables**

</aside>

- ***Declaration*:**
    - A variable in Java must be declared before it can be used.
    - The declaration includes data type and name of variable.
        
        ```java
        int number;
        ```
        
    - In this example, **`int`** is the data type and **`number`** is the name of the variable.
- ***Initialization*:**
    - We can also initialize a variable at time of declaration or later.
        
        ```java
        int number = 10;
        ```
        

<aside>
💡 **Types of Variables**

</aside>

- There are **3 types** of variables in Java →
    1. ***Local Variables:*** These are declared within a block, method, or constructor. They are created when block is entered or function is called, and destroyed after exiting from block or when the call returns from the function.
        
        ```java
        public void myMethod() {
            int localVariable = 10; // This is a local variable
        }
        ```
        
    2. ***Instance Variables:*** These are declared inside the class but outside any method. They are not declared as static. Each instance of the class has its own copy of the instance variable.
        
        ```java
        public class MyClass {
            int instanceVariable; // This is an instance variable
        }
        ```
        
    3. **Static Variables**: These are declared as static. They cannot be local. There is only one copy of a static variable, and it is shared among all instances of the class.
        
        ```java
        public class MyClass {
            static int staticVariable; // This is a static variable
        }
        ```
        
- *Example*:
    
    ```java
    public class Main {
        static int staticVariable = 100; // Static variable
        int instanceVariable = 200; // Instance variable
    
        public void myMethod() {
            int localVariable = 300; // Local variable
            System.out.println("Local variable: " + localVariable);
            System.out.println("Instance variable: " + instanceVariable);
            System.out.println("Static variable: " + staticVariable);
        }
    
        public static void main(String[] args) {
            Main obj = new Main();
            obj.myMethod();
        }
    }
    
    ```
    

<aside>
💡 **Data Types**

</aside>

- Variables in Java can be of **2 data types**:
    - ***Primitive Data Types:***
        
        They are predefined and of **8 types**: 
        
        1. `**byte**`: Size is 8-bit / 1 byte. Its a signed two’s complement (positive, negative and zero) integer. Minimum value of -128 & maximum value of 127.
            
            ```java
            byte b = 10; // Example of byte
            ```
            
        2. `**short**`: Size is 16-bit / 2 byte. A signed two’s complement integer. Minimum value of -32,768 & maximum value of  32,767.
            
            ```java
            short s = 10000; // Example of short
            ```
            
        3. `**int**`: Size is 32-bit / 4 byte. A signed two’s complement integer. Minimum value of -2,147,483,648 (-2^31) & maximum value of 2,147,483,647 (2^31 -1). 
            
            ```java
            int i = 100000; // Example of int
            ```
            
        4. `**long**`: Size is 64-bit / 8 byte. A signed two’s complement integer. Minimum value of -9,223,372,036,854,775,808 (-2^63) & maximum value of 9,223,372,036,854,775,807 (2^63 -1). 
        
        ```java
        long l = 100000L; // Example of long
        ```
        
        1. `**float**`: This is a signed & single-precision (less accurate) 32-bit / 4 bytes IEEE 754 floating point. 
            
            ```java
            float f = -20.0f; // Example of float
            ```
            
        2. `**double**`: This is a signed & double-precision 64-bit / 8 bytes IEEE 754 floating point. 
            
            ```java
            double d = 30.0; // Example of double
            ```
            
        3. `**boolean**`: This data type represents 1 bit of information, but its size isn’t precisely defined.
            
            ```java
            boolean bool = true; // Example of boolean
            ```
            
        4. `**char**`: This is a single 16-bit / 2 bytes Unicode character. 
            
            ```java
            char c = 'a'; // Example of char
            ```
            
    - ***Non-primitive Data Types:***
        
        They are programmer defined: **`String`**, **`Array`**, **`Class`**, **`Interface`**, etc.
        
- *Example:*
    
    ```java
    public class Main {
        public static void main(String[] args) {
            boolean bool = true;
            byte b = 10;
            char c = 'a';
            short s = 10000;
            int i = 100000;
            long l = 100000L;
            float f = 20.0f;
            double d = 30.0;
            String str = "Hello, World!";
            
            System.out.println("boolean: " + bool);
            System.out.println("byte: " + b);
            System.out.println("char: " + c);
            System.out.println("short: " + s);
            System.out.println("int: " + i);
            System.out.println("long: " + l);
            System.out.println("float: " + f);
            System.out.println("double: " + d);
            System.out.println("String: " + str);
        }
    }
    ```
    

<aside>
💡 **Primitive Data Types**

</aside>

- 

<aside>
💡 **Rules**

</aside>

- Code must start with a `public class`, and that **class name** should be **same** with **file name**
- We can’t use **[main](https://www.notion.so/JAVA-Full-Notes-a157d095d55c493fbe49d9357ddf0086?pvs=21)** or any other inbuilt keyword anywhere in Java code
-

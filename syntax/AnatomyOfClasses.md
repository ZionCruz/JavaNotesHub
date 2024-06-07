<h1 align="center">Anatomy of Classes</h1>
<br></br>

## Main Class Structure:
In Java, the main class is where the program starts its execution. It contains the main method, which serves as the entry point for the **Java Virtual Machine (JVM)** to begin executing the program. Here's the basic structure of a main class:

```
public class Main {
    public static void main(String[] args) {
        // Program logic goes here
    }
}
```
### Explanation:
1. **Class Declaration:**
    - The keyword **class** is used to declare a new class in Java. In this case, we have a class named **Main**.

2. **Main Method** 
    - The **main** method is the entry point for the Java program. It has a specific signature:
        - **_public:_** It is acessible from anywhere.
        - **_static:_** It belongs to the class, not an instance of the class.
        - **_void:_** It does not run any value.
        - **_main:_** It is the name of the method.
        - **_string[] args:_** It takes an array of strings as input parameters. These parameters can be used to pass command-line arguments to the program.

3. **Program Logic**
    - Inside the **main** method, you write the logic for your program. This is where you define what the program should do when it starts executing.

-----

#### There are also important points to pay attention to:
- Most of our classes will start with public class;
- Every class needs a name, for example MyClass;
- The file name needs to be identical to the public class name;
- Within an application, it is recommended that only one class has the main method, responsible for starting our entire program;
- The main method is named main, always has public visibility, is defined as static, does not return any value with void, and receives a parameter of type String array String[].

<br></br>

## Naming Conventions:

Naming conventions, are guidelines used to name classes, variables, methods, and other elements in a program consistently. Following a consistent naming convention makes your code more readable and understandable for yourself and others who may work with your code. Here are some common naming conventions used in Java:

1. **Class Names**
    - Start with an uppercase letter.
    - Use nouns or noun phrases that describe the class's purpose.
    - Use camel case, where each word starts with an uppercase letter (e.g., ClassName).
    - The class must have the same name as the file.java, for example:

```
// ScientificCalculator.java file

public class ScientificCalculator {

}
```

2. **Variable Names**
    - Start with a lowercase letter;
    - Use meaningful names that describe the variable's purpose;
    - Use camel case;
    - It must contain only letters, _ (underscore), $ or numbers from 0 to 9;
    - It must necessarily start with a letter (preferably), _ or $, never with a number;
    - It cannot contain spaces;
    - We cannot use language keywords;
    - The name must be unique within a scope.

```
// Invalid variable declarations

int number&one = 1; // The only allowed symbols are _ and $
int 1number = 1;   // A variable cannot start with a number
int number one = 1; // A variable name cannot contain spaces
int long = 1;      // long is a reserved keyword in the language

// Valid variable declarations
int number$one = 1;
int number1 = 1;
int numberone = 1;
int long1 = 1;
```

---
<br></br>

## Declaring Variables:

**Syntax:**
```
dataType variableName;
dataType variableName = value; // Declaration with initialization
```
**Examples:**
```
int number;                   // Variable declaration
int age = 25;                 // Variable declaration with initialization
String name = "John";         // Reference variable declaration with initialization
double salary = 50000.00;     // Variable declaration with initialization
boolean isActive = true;      // Variable declaration with initialization
```
---
## Declaring Methods:
**Syntax:**
```
accessModifier returnType methodName(parameters) {
    // Method body
}
```

**Examples:**
```
//Method with No Parameters and No Return Value:
public void printHello() {
    System.out.println("Hello, World!");
}


//Method with Parameters and No Return Value:
public void greet(String name) {
    System.out.println("Hello, " + name);
}


//Method with Parameters and a Return Value:
public int add(int a, int b) {
    return a + b;
}


//Method with No Parameters and a Return Value:
public String getGreeting() {
    return "Hello, World!";
}
```

## Identifying the Difference Between Variables and Methods:

**Variables:**
- Store data values.
- Have a data type (e.g., int, String, boolean).
- Declared inside a class, method, or block.
- Can be identified by their declaration syntax (dataType variableName).

**Methods:**
- Perform actions or operations.
- Have a return type, method name, and a parameter list (if any).
- Declared inside a class.
- Can be identified by their method signature (returnType methodName(parameters)).

### Common Structure for Both:

**Variables:**
- Usually declared at the beginning of a class or method.
- Can have modifiers like _public_, _private_, _protected_, _final_, _static_.
- Commonly follow camelCase naming convention.

**Methods:**
- Declared inside a class.
- Have a return type, name, and parameter list.
- Method body enclosed in {}.
- Can have modifiers like _public_, _private_, _protected_, _static_, _final_.
- Follow camelCase naming convention.
---

<br></br>
## Identation:

Indentation is the practice of adding consistent spacing at the beginning of lines of code to visually organize and structure your code. It's not a requirement for the compiler, but it's essential for readability and maintainability, especially in languages like Java where indentation doesn't affect the program's logic. Here are some key points about indentation:

Importance of Indentation:
- Readability: Proper indentation makes code easier to read and understand, both for yourself and for others who may work with your code.

- Structure: Indentation visually represents the structure of your code, making it clear which statements are contained within which blocks of code (e.g., loops, conditionals, methods).

- Debugging: Indentation helps identify syntax errors and logical mistakes more quickly by highlighting the structure of your code.

### Common Indentation Practices:

1. Consistency: Use the same indentation style throughout your codebase. Common choices include using spaces or tabs, and typically, each indentation level is 2 to 4 spaces or one tab.

2. Block Indentation: Indent blocks of code enclosed within curly braces {}. This includes the body of methods, loops, conditionals, and class definitions.

3. Alignment: Align related code elements vertically to improve readability. For example, aligning variable declarations or method parameters.

**Example of Poor Indentation:**
```
public class BadIndentationExample{
public static void main(String[] args){
int number=10;
if(number>5){
System.out.println("Number is greater than 5.");
}else{System.out.println("Number is less than or equal to 5.");}
for(int i=0;i<5;i++){
System.out.println("Iteration "+(i+1));}}
}
```

**Example of Proper Indentation:**
```
public class Example {
    
    public static void main(String[] args) {
        int number = 10;
        
        if (number > 5) {
            System.out.println("Number is greater than 5.");
        } else {
            System.out.println("Number is less than or equal to 5.");
        }
        
        for (int i = 0; i < 5; i++) {
            System.out.println("Iteration " + (i + 1));
        }
    }
}
```
---
<br></br>

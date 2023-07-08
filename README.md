# Rust Programming

## What is programming?

Computer programming is the process of writing code that instructs how a computer, application or software program performs.
At its most basic, computer programming is a set of instructions to facilitate specific actions.

## What is Rust?
Rust is a multi-paradism, general-purpose programming language designed for performance and safety, especially safe concurrency.
Rust is a system level programming language, developed by Graydon Hoare. Mozilla Labs acquired the programme.

# What is system programming?
Systems programming language like C/C++ are used to build software and software platforms. They can be used to build operaing system, game engines, compilers, etc.
Systems and application programming language face two major problems -
1. It is difficult to write secure code.
2. It is difficult to write multi-threaded code.

## Why Rust?
Rust focuses on three goals:
1. Speed
2. Safety
3. Concurrency

The language was designed for developing highly reliable and fast software in a simple way. Rust can be used to write high-level programs down to hardware-specific programs.

## Performance
Rust programming language does not have a Garbage Collector (GC) by design. This improves the perfomance at runtime.

## Memory safety at compile time
Software build using Rust is safe from memory issues like dangling pointers, buffer overruns and memory leaks.

## Multi-threaded applications
Rust ownership and memory safely rules provide concurrency without data races.

## Supports for web Assembly (WASM)
Web Assembly helps to execute high computation intensive algorithms in the browser, on embedded devices, or anywhere else. It runs at the speed of native code. Rust can be compiled to Web Assembly for fast, reliable execution.

# Installation

## Using linux ubuntu system
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

## Configure the PATH environment variable
```
~/.cargo/bin
```
 Based on installed dependencies folder

## Check version
```
rustc --version
```

# Comments and Print Statements

## Comments
Comments are the statements that are used for documentation purpose or Comments are ignored by compiler so that don't execute.

Thare are two types of comments in Rust:
1. Single line comment. [//]
2. Multi line comment. [/* */]
Multi line comment is used for commenting multiple line of statement

## Print Statement
1. Println!() -> for a new line
2. Print!() -> no new line

## Example
```
fn main(){
    /* This 
    is
    my
    name */
    println!("Hello");
    println!("Anurag");
    // This is single line comment
    print!("Hello");
    print!("Anurag");
}
```

# Variables

## What are variables?
Variables are the name you give to computer memory locations which are used to store values in a computer program.

For example, assume you want to store two values 10 and 20 in your program and at a later stage, you want to use these two values. Let's see how you will do it. Here are the following three simple steps :-
1. Create variables with appropriate names.
2. Store you values in those two variables.
3. Retrieve and use the stored values from the variables.

## Creating variables
Creating variables is also called declaring variables in Rust programming.
Use the let keyword to declare a variable.

### Example
```
fn main(){
    let name = "charVariable";
    let num = 100;
    let floatNum = 2.5;
    let boolValue = True;
    println!("Character variable is {}", name);
    println!("Number variable is {}", num);
    println!("Float variable is {}", floatNum);
    println!("Boolean variable is {}", boolValue);
}
```

The println! takes two arguments:-
1. A special syntax {}, which is the placeholder
2. The variable name or a constant
3. The placeholder will be replaced by the variable's value

## Syntax
1. The data type is optional while declaring a varible in Rust. The data type is inferred from the value assigned to the variable.
2. The syntax for declaring a variable is given below.
```
let variable_name = value // no type specified
let variable_name:dataType = value // type specified
```

# Naming Convention & Keywords in Rust

## What is keywords?
Keywords are predefined, reserved words used in programming that have special meanings to the compiler. Keywords are part of the syntax and they cannot be used as an identifier.

### The following keywords currently have the functionality described
* **as**- perform primitive casting, disambiguate the specific trait containing an item, or rename items in use and external create statements
* **async**- return a Future instead of blocking the current thread
* **await**- suspend execution until the result of a Future is ready
* **break**- exit a loop immediately
* **const**- define constant items or constant raw pointers
* **continue**- continue to the next loop iteration
* **crate**- link an external crate or a macro variable representing the crate in which the macro is defined
* **dyn**- dynamic dispatch to a trait object
* **else**- fallback for if and if let control flow constructs
* **enum**- define an enumeration
* **extern** link an external crate, function, or variable
* **false**- Boolean false literal
* **fn**- define a function or the function pointer type
* **for**- loop over items from an iterator, implement a trait, or specify a higher-ranked lifetime
* **if**- branch based on the result of a conditional expression
* **impl**- implement inherent or trait functionality
* **in**- part of for loop syntax
* **let**- bind a variable
* **loop**- loop unconditionally
* **match**- match a value of patterns
* **mod**- define a module
* **move**- make a closure take ownership of all its captures
* **mut**- denote mutability in references, raw pointers, or pattern bindings
* **pub**- denote public visibility in struct fields, impl blocks, or modules
* **ref**- bind by reference
* **return**- return from function
* **Self**- a type alias for the type we are defining or implementing
* **self**- method subject or current module
* **static**- global variable or lifeime lasting the entire program execution
* **struct**- define a structure
* **super**- parent module of the current module
* **trait**- define a trait
* **true**- Boolean true literal
* **type**- define a type alias or associated type
* **union**- define a union and is only a keyword when used in a union declaration
* **unsafe**- denote unsafe code, functions, traits, or implementations
* **use**- bring symbols into scope
* **where**- denote clauses the constrain a type
* **while**- loop conditionally based on the result of an expression

## Keyword reserved for future use
### The following keywords do not have any functionality but are reserved by Rust for potential future use
* **abstract**
* **become**
* **box**
* **do**
* **final**
* **macro**
* **override**
* **priv**
* **try**
* **typeof**
* **unsized**
* **virtual**
* **yield**

## Naming conventions What are they?
Naming conventions are rules that dictate the way you name the various files, folders, and tokens in our code (such as variables, functions, and so on).

The entire idea behind naming conventions is to help make code more maintainable for the reader. By enforcing a convention and naming tokens consistently, we accomplish two things: discoverability and understanding

**Discoverability**- How quickly can someone find a folder, file, feature, or method they need to change.
**Understanding**- How fast can someone look at our code and understand what it is they're looking at.

## Rust for naming in Rust
* The name of a varible can be composed of letters, digits, and the underscore character.
* It must be begin with eiter a letter or an underscore.
* Upper and lowercase letters are distinct because Rust is case-sensitive.

## The common naming conventions for Rust
1. Camel case (ex: someVariable)
2. Snake case (ex: some_variable)

### Example
```
let someVarible = "anurag";
let another_variable = 20;
println!("Camel case variable is {}": someVariable);
println!("Snake case variable is {}": another_variable);
```

# Data Types in Rust

## What are data-types?
The data type of a value (or variable in some contexts) in an attribute that tells what kind of data that value can have.
In simple words it is value of a varibale

### Data types in Rust are divided into different groups:
* **Scalar Type**
* **Compound Type**

## Scalar Type
A scalar type represents a single value. Rust has four primary scalar type.
* **Integer**
* **Floating-point**
* **Boolean**
* **Character**

### Integer
An integer is a number without a fractional component. Integer can be further classified as Signed and Unsigned. Signed integers can store both negative and positive values. Unsigned integer can only store positive values. **Integer is i32 by default**
```
size        Signed  Unsigned
8 bit        i8      u8
16 bit      i16      u16
32 bit      i32      u32
64 bit      i64      u64
128 bit     i128     u128
Arch        Isize    usize
```
Each signed variant can store numbers from -(2^n-1) to 2^n-1 inclusive, where n is the number of bits that variant uses. So an i8 can store numbers from -(2^7) to 2^7-1, which equal to -128 to 127. Unsigned variants can store numbers from 0 to 2n-1, so a u8 can store numbers from 0 to 2^8, which equal 0 to 155.
Additionally, the isize and usize types depend on the architecture of the computer your program is running.

### Floating-point Types
Rust also has two primitive types for floating-point numbers, which are numbers with decimal points. Rust's floating-point types are f32 and f64, which are 32 bits and 64 bits in size, resp. The **default type is f64** because on modern CPUs it's roughly the same speed as f32 but is capable of more precision. All floating point types are signed.
The f32 type is a single-precision float, and f64 has double precision.

### Boolean
Boolean types have two possible value- true or false. Use the bool keyword to declare a boolean variable.

### Character
The character data type in Rust supports numbers, alphabets, Unicode and special character. Use the char keyword to declare a variable of character data type.

**Note** that we specify char literals with single quotes, as opposed to string literals, which use double quotes. Rust's char type is four bytes in size and represents a Unicode Scalar value, which means it can represent a lot more than just ASCII. Accented letters; Chinese, Japenese, and Korean characters; emoji; and zero-width spaces are all valid char values in Rust.

### Automatic Type casting
Automatic type casting is not allowed in Rust.

### Number Separator
For easy readabilit of large numbers, we can use a visual separator_underscore to separate digits. That is **50000 can be written as 50_000**.

## Example
```
fn main(){
    let _name:char = 'a';
    let emoji_char = '😁'
    let _num:i8 = 10_000; // means value is 10,000
    let _float:i8 = 1.5;
    let _bool:bool = true;
}
```
# Mutable & Immutable

## Immutable
By default, variables are immutable. In other words, the variable's value cannot be changed once a valid is defined.

## Mutable
**Variables are immutable by default**. Prefix the variable name with **mut** keyword to make it mutable. The value of a mutable variable can be changed.

### Example
```
fn main(){
    let mut amount:i32 = 20_000;
    println!("Amount is {}", amount);
    amount = 25_000;
    println!("Amount is {}", amount);
}
```
* **Immutable**- cannot change the value
* **Mutable**- change the value stored

# Constants in Rust
## Constants
Constants represent values that cannot be changed. If you declare a constant then there is no way its value change. The keyword for using constants is **const**.
The naming convention for Constants are similar to that of variables. All characters in a constant name are usually in uppercase.

## Constant vs Variable
* Constants are declared using the **const** keyword while variables are declared using the let keyword.
* A variable declaration can optionally have a data type whereas a constant declaration must specify the data type. This means const **USER_LIMIT=100** will result in an error.
* A variable declared using the **let** keyword is by default immutable. However, you have an option to mutate it using the mut keyword. Constants are immutable.
* Constants can be set only to a constant expression and not to the result of a function call or any other value that will be computed at runtime.
* Constants can be declared in any score, including the global scope, which makes them useful for values that many parts of the code need to know about.

### Example
```
fn main(){
    let mut num:i8 = 10;
    println!("{}", num);
    const PIE:f8 = 3.75;
    println!("Constant value is {}", PIE);
    PIE = 4.5; // through error
    println!("Constant value is {}", PIE);
}
```

# Literals and Casting in Rust

## Literals
A literal is a notation for representing a fixed value in a variable.
Numeric literals can be type annotated by adding the type as a suffix. As an example, to specigy that the literal 42 should have the i32, **write 43i32**.
The type of unsuffixed numberic literals will depend on how they are used. If no constraint exists, the compiler will use i32 for integers, and f64 for floating-point numbers.

### Example
```
fn main(){
    // Suffixed literals, their types are known at initialization
    let x = 1u8;
    let y = 2u16;
    let z = 30u32;

    // Unsuffixed literals, their types depend on how they are use
    let i = 1;
    let f = 1.0;
}
```

## Casting
The conversion of one data type into another.
Rules for converting between different types. In Rust, we make use of **as** keyword when we want to convert from ont type to another.

### Example
```
fn main(){
    let decimal_value = 5.6_f32;
    let int_value = decimal_value as i8;
}
```

# Operators in Rust

## Operators
An operator is a symbol that tells the compiler to perform specific mathematical operation and produce final result
```
Operant     Operator      Operand
1              +            2
```

### The following are the types of operators in Rust:
* **Arithmetic Operators**
* **Comparison Operators**
* **Logical Operators**
* **Bitwise Operators**
* **Compound Assignment Operators**

## Arithmetic Operators
Arithmetic operators are used for performing mathematical operations like addition, substraction, multiplication, and division.
```
Operator    Explanation                                                                     Example
+           Returns the addition of two operands                                            A+B = 10
-           Returns the difference of the values (subtract right operand from left)         A-B = 23
*           Returns the product of the values                                               A*B = 100
/           Divide left operand by right one and returns the quotient                       A/B = 3
%           Divide left operand by right one and returns the remainder                      A%B = 9
```

## Comparison Operators
Comparison operators are the operators that compare value and return true or false depending upon the conditions.
```
Operator        Explanation                 Example
>               Greater than                (A+B) is true
<               Less than                   (A<B) is false
==              Equal to                    (A==B) is false
!=              Not equal to                (A!=B) is true
>=              Greater than and equal to   (A>=B) is true
<=              Less than and equal to      (A<=B) is false
```

## Logical Operators
Logical operators are used to combine two or more conditions. Logical operators too, return a Boolean value.
```
Operator    Explanation
&&          The operator returns true only if all the expressions specified return true 
||          The operator returns true if at least one of the expressions specified return true
!           The operator returns the inverse of the expression’s result
```

## Compound Assignment Operator
Compound assignment operators perform the operation specified by the additional operator, then assign the result to the left operant.
```
Operator    Explanation
+=          Arithmetic addition and assignment
-=          Arithmetic subtraction and assignment
*=          Arithmetic multiplication and assignment
/=          Arithmetic division and assignment
%=          Arithmetic remainder and assignment
```

# String in Rust

## String
Strings are sequence of characters.
The string in rust can be classified into the two ways:
* **String literal (&str)**
* **String Object (String)**

### String literal
String literal (&str) are used when the value of a string is known at compile time. String literals are a set of characters, which are hardcoded into a variable.
```
fn main(){
    let name:&str = "stringValue";
    println!("{}", name);
}
```
String literals are static by default. This means that string literals are guaranteed to be valid for the duration of the entire program.

### String object
To create a String object, we can use any of the following syntax:-
* **String::new()**
* **String::from()**
This creates a string with some default value passed as parameter to the form() method.

## String slicing
String slicing is all about fetching a substring (part of a string) from a given string.
Therefore, we need to specify the starting and ending index of a string. **Index start from 0**.

The minimum index value is 0 and the maximum index value is the size of the data structure.
**NOTE** that the last index not be include in the final string.

The diagram below shows a sample string Anurag, that has 8 characters. The index of the first character is 0 and that of the last character is 5.
```
A   N   U   R   A   G
0   1   2   3   4   5
```
### Example
```
fn main(){
    let name = "Anurag"
    let n = &name[0:2];
    println!("{}", n);
}
```
## String concatenation
1. **Format!()**
2. **+**

### Format!()
We can use it for both string literals and string object
```
fn main(){
    let name = "Anurag";
    let name_2 = "Saini";
    let full_name = format!("{} {}", name, name_2);
    println!("{}", full_name);
}
```
### +
Only used for string object
```
fn main(){
    let first_name = "Anurag".to_string();
    let last_name = "Saini".to_string();
    let full_name = first_name+last_name;
    println!("{}", full_name);
}
```
## String methods
Methods are used for checking and modifying the string.

* **new()**- Creates a new empty string.
* **from()**- Creates a new string having default value.
* **to_string()**- Converts string literal to string object.
* **replace()**- Replaces all matches of a pattern with another string.
* **push()**- Appends the given char to the end of this string.
* **push_str()**- Appends a given string into the end of this string.
* **len()**- Returns the length of the string.

# Escape Sequence in Rust

## Escape Sequence
An escape sequence is a sequence of characters that does not represent itself when used inside string literal, but is translated into another character or a sequence of characters that may be difficult or impossible to represent directly.

### Important Escape Sequence
```
Escape   sequence Description
\n       New line
\t       Tab
\\       Insert backslash
\r       Start from initial point
\’       Insert single quote
\”       Insert double quote
```

# Decision Making in Rust

## Decision Making
Decision making structures require that the programmer specify one or more conditions to be evaluated or tested by the program, along with a statement or statements to be executed if the condition is determined to be true, and optionally, other statements to be executed if the condition is determined to be false.

### Type of Decision making statements
1. **if...else**
2. **else...if**
3. **match statement**

## if...else
An if statement can be followed by an optional else statement, which executes when the Boolean expression is false. If the Boolean expression evalutes to true, then the if block will be executed, otherwise, the else block will be executed.
```
fn main(){
    let num = 19;
    let num2 = 20;
    if num == num2 {
        println!("Both value are same");
    } else {
        println!("Value not same");
    }
}
```

## else...if
The else...if ladder is useful to test multiple conditions
```
fn main(){
    let num = 10;
    let num2 = 20;
    if num == num2 {
        println!("Both are same");
    } else if num < num2 {
        println!("Number 2 is greater");
    } else {
        println!("Number 1 is greater");
    }
}
```
## Match statement
The match statement checks if a current value is matching from a list of value.
```
fn main(){
    let num = 4;
    match num{
        1 => println!("One"), // match a single value
        2 | 3 | 4 => println!("Number in between 2 to 4"), // match several value
        5..=10 => println!("Number in range 5..10"), // match an inclusive range
        _ => println!("not specify"), // handle the defalut or rest case
    }
}
```

# Loops in Rust

## Loop
A loop is a sequence of instruction's that is continually repeated until a certain condition is reached.

### Types of loops in rust
* **while**
* **for**
* **loop**

## For loop
**for** loop executed the code block for a specified number of times. It can be used to iterate over a fixed set of values, such as array.
```
for x in 1..10{
    println!("{}", x);
}

// x is range of 1 to 10, where 1 is implicit and 10 is explicit. If you want to include 10th value also use **for x in 1..=10**
```

## loop
**loop** is not a conditional loop. It is keyword that tells the **rust** to exeecute the block of code over again and again until and unless you explicity stop the loop manually.
```
loop{
    println!("Hi Anurag!");
}
```

## While loop
**while** loop is a conditional loop. When a program needs to evaluate a condition than the conditional loop is used. When the condition is true then it executes the loop otherwise it terminates the loop.
```
fn main(){
    let mut x=1;
    while x<10 {
        println!("{}", x);
        x+=1'
    }
}
```

## Difference between while loop and for loop
If the index length of the array is increased at runtime, then the while loop shows the bug this would not be happened in the class of for loop. Therefore, we can say that for loop increases the safety of the code and removes the changes of the bugs.

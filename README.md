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

# COMMENTS AND PRINT STATEMENT

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


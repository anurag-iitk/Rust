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
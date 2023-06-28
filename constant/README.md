# Constants in Rust

## Constants
Constants represent values that cannot be changed. If you declare a constant then there is no way its value change. The keyword for using constants is **const**.
The naming convention for Constants are similar to that of variables. All characters in a constant name are usually in uppercase.

## Constant vs Variable
* Constants are declared using the **const** keyword while variables are declared using the let keyword.
* A variable declaration can optionally have a data type whereas a constant declaration must specify the data type. This means const **USER_LIMIT=100** will result in an error.
* A variable declared using the **let**keyword is by default immutable. However, you have an option to mutate it using the mut keyword. Constants are immutable.
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
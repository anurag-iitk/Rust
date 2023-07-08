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
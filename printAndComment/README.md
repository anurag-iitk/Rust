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


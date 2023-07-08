# User Input in Rust
User input is most important an any of the programming language. They helps to interact the application.

## Example
```
fn main(){
    // create a empty string
    let mut _value = String::new();
    println!("Enter the value: ");
    // user input in string value
    let _v = std::io::stdin().read_line(&mut _value).unwrap();
    println!("{}", _value);

    // Change **String** to **int**
    let _i: i32 = _value.trim().parse().expect("Value not integer");
    println!("{}", _x);
}
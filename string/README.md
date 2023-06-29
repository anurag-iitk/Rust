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

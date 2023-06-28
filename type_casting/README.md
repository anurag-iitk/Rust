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
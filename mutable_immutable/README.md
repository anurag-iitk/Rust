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
**Immutable**- cannot change the value
**Mutable**- change the value stored

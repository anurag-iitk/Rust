# Tuple in Rust
A finite series of different datatype.

## Example
```
fn main(){
    // for store same type
    let _t1 = 12, 23;
    let _t2:(i32, f32, bool, char, &'static str) = (10, 10.5, false, 'a', "hi");
    println!("{:?}", _t2);

    asset_eq!(_t2.0, 10)
    println!("{:?}", _t2.0);
    println!("{:?}", _t2.1);
}
```

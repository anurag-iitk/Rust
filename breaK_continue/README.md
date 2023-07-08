# Break and Continue in Rust

## Break Keyword
When **break** is executed, it immediately terminates the loop body.
```
fn main(){

    let mut _value = 0;

    for x in 1..10 {
        if x > 5 {
            break;
        }
        _value = x;
    }

    println!("{}", _value);
}
```

## Continue Keyword
When **continue** is executed, mainly skip running iteration and move to next iteration.
```
fn main(){
    for number in 1..=10 {
        if number % 2 == 0 {
            continue;
        }
        println!("Only odd numbers: {number}");
    }
}
```

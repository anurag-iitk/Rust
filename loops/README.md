# Loops in Rust

## Loop
A loop is a sequence of instruction's that is continually repeated until a certain condition is reached.

### Types of loops in rust
* **while**
* **for**
* **loop**

## For loop
**for** loop executed the code block for a specified number of times. It can be used to iterate over a fixed set of values, such as array.
```
for x in 1..10{
    println!("{}", x);
}

// x is range of 1 to 10, where 1 is implicit and 10 is explicit. If you want to include 10th value also use **for x in 1..=10**
```

## loop
**loop** is not a conditional loop. It is keyword that tells the **rust** to exeecute the block of code over again and again until and unless you explicity stop the loop manually.
```
loop{
    println!("Hi Anurag!");
}
```

## While loop
**while** loop is a conditional loop. When a program needs to evaluate a condition than the conditional loop is used. When the condition is true then it executes the loop otherwise it terminates the loop.
```
fn main(){
    let mut x=1;
    while x<10 {
        println!("{}", x);
        x+=1'
    }
}
```

## Difference between while loop and for loop
If the index length of the array is increased at runtime, then the while loop shows the bug this would not be happened in the class of for loop. Therefore, we can say that for loop increases the safety of the code and removes the changes of the bugs.

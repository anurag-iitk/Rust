# Rust Programming

## What is programming?

Computer programming is the process of writing code that instructs how a computer, application or software program performs.
At its most basic, computer programming is a set of instructions to facilitate specific actions.

## What is Rust?
Rust is a multi-paradism, general-purpose programming language designed for performance and safety, especially safe concurrency.
Rust is a system level programming language, developed by Graydon Hoare. Mozilla Labs acquired the programme.

# What is system programming?
Systems programming language like C/C++ are used to build software and software platforms. They can be used to build operaing system, game engines, compilers, etc.
Systems and application programming language face two major problems -
1. It is difficult to write secure code.
2. It is difficult to write multi-threaded code.

## Why Rust?
Rust focuses on three goals:
1. Speed
2. Safety
3. Concurrency

The language was designed for developing highly reliable and fast software in a simple way. Rust can be used to write high-level programs down to hardware-specific programs.

## Performance
Rust programming language does not have a Garbage Collector (GC) by design. This improves the perfomance at runtime.

## Memory safety at compile time
Software build using Rust is safe from memory issues like dangling pointers, buffer overruns and memory leaks.

## Multi-threaded applications
Rust ownership and memory safely rules provide concurrency without data races.

## Supports for web Assembly (WASM)
Web Assembly helps to execute high computation intensive algorithms in the browser, on embedded devices, or anywhere else. It runs at the speed of native code. Rust can be compiled to Web Assembly for fast, reliable execution.

# Installation

## Using linux ubuntu system
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

## Configure the PATH environment variable
```
~/.cargo/bin
```
 Based on installed dependencies folder

## Check version
```
rustc --version
```

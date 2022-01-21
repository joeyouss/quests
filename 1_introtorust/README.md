Rust:
- installing rust -> install Rustup (version management tool) -> because Rust has too many releases
- command: `curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`
- checking commands: `which cargo` and `which rustc`
- dependecies in rust are managed thru a file named `cargo.toml`
- extensions to download: rust and crates.
- create a new folder: `cargo new hello-world --bin`
- hello-world/cargo.toml: contains metadata about the app
- src: folder which contains application code
- entry point to app is always name `main.rs`
- macros are functions which write more code
- run the file: `cargo run`
- post compilation: binary created in `target` folder

variables and immutability:
- boxes which hold some value
- keyword: `let`
- variables CANNOT be reassigned
- to make variables changeable: use the keyword `mut` to make it mutable

types:
- annotating a type: add a `:` and then the type
- example: let x: i32=5;
- type inference: rust compiler assumes the type of the variable

composite types:
- tuples: return a set of values of different types
- dot operator instead of brackets
- destructuring: let(one,two,three) = a
- arrays: use square brackets
- fill array with zeroes: let arr = [0;10];

control flow:

```
let num=1;
if num==1{
    println!("you won"!);
}
else{
    println!("you lost");
}
````

Loops:
- multiply a number till < 5000
```
let mut x = 1;
loop{
    x = x*2;
    if x>5000{
        break;
    }
    println!("{}", x);
}
```

- for :
```
for x in 0...10{
    println!("{}", x)
}
```


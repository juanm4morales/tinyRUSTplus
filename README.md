# tinyRust+ compiler

**tinyRust+** is an academic project aimed at reinforcing programming skills and fostering the understanding of advanced concepts, particularly in object-oriented programming (OOP). It takes Rust as a foundation—well-known for its memory safety and runtime efficiency—but challenges the conventional notion of Rust by integrating a more traditional OOP approach. 

## Table of Contents
1. [Language Features](#language-features)  
2. [Installation](#installation)
3. [Usage](#usage)
5. [Example Code](#example-code)
6. [License](#license)

---

## Language Features

tinyRust+ is an object-oriented language with the following features:

- **Strong and static typing**: All variables have an associated data type that is checked at compile time.
- **Class-based organization**: Allows defining classes that can inherit attributes and methods from other classes.
- **Method inheritance and overriding**: Non-static inherited methods can be overridden, but attributes cannot.
- **Polymorphism**: Objects of different classes can be instantiated and used polymorphically.
- **Encapsulation**: Attribute visibility levels can be defined within a class.
- **`main` method as the entry point**: Every program must contain a `main` method, declared outside the scope of classes.
---

## Installation

To set up and run the tinyRust+ compiler, follow these steps:

1. Clone the repository:
   ```sh
   git clone https://github.com/user/tinyRUSTplus.git
   ```
2. Open Eclipse and import the project:
   - Select **File > Import > Existing Projects into Workspace**.
   - Choose the cloned repository folder.
   - Click **Finish** to import the project.
3. Generate the JAR file:
   - Click **File > Export > Java > Runnable JAR file**.
   - Select the `Runner` class as the launch configuration.
   - Choose an export destination (e.g., `tinyRUSTplus.jar`).
   - Click **Finish** to generate the JAR file.


## Usage

To compile a tinyRust+ source file, use the following command:
```sh
java -jar tinyRUSTplus.jar <SOURCE_FILE>.ts
```
This will generate an equivalent MIPS32 assembly code.

## Example Code

```rust
class Fibonacci {
    pub I32: suma;
    I32: i,j;
    fn sucesion_fib(I32: n)-> void{
        I32: idx;
        i=0; j=1; suma=0; idx = 0;
        while (idx <= n){
            (out_idx(idx));
            (out_val(i));
            suma = i + j;
            i = j;
            j = suma;
            idx = idx + 1;
        }
    }
    create(){
        i=0;
        j=0;
        suma=0;
    }
    fn out_idx(I32: num) -> void{
        (IO.out_str("f_"));
        (IO.out_i32(num));
        (IO.out_str("="));
    }


    fn out_val(I32: s) -> void{
        (IO.out_i32(s));
        (IO.out_str("\n"));
    }
}
fn main(){
    Fibonacci: fib;
    I32: n;
    fib = new Fibonacci();
    n = IO.in_i32();
    (fib.sucesion_fib(n));
}
```


## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.


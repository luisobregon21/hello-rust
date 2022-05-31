# Learning Rust

## Generating a New project

To create a new project, run the following command:

```cargo new projectName```

That generates a new project with the name that was assigned and the following files. 

```shell
hello-rust
|- Cargo.toml
|- src
  |- main.rs
```

```Cargo.toml``` is the manifest file for Rust. It’s where you keep metadata for your project, as well as dependencies.

```src/main.rs``` is where we’ll write our application code.

```cargo new``` generates a "Hello, world!" project for us! We can run this program by moving into the new directory that we made and running this in our terminal:

```cargo run``` which shows:

```shell
$ cargo run
   Compiling hello-rust v0.1.0 (/Users/ag_dubs/rust/hello-rust)
    Finished dev [unoptimized + debuginfo] target(s) in 1.34s
     Running `target/debug/hello-rust`
Hello, world!
```

## Dependacies

package registry for Rust: [creates.io](https://crates.io)

In ```Cargo.toml```, under depandacies, you can add packages aka "crates".

```Rust
[dependencies]
ferris-says = "0.2"
```

And then run ```cargo build``` to install the dependacies.

```cargo.lock``` is a log of the exact versions of the dependencies we are using locally.

### Using Dependacy

in a file like ```main.rs``` add the line...

```Rust
 use ferris_says::say;
 ```

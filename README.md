# Minigrep 

A simple command-line text search tool built in Rust, inspired by the `minigrep` project from [The Rust Programming Language Book](https://doc.rust-lang.org/book/).

The program takes a search query and a file path as command-line arguments, reads the file, and prints the lines containing the search query.

## Features

- Accepts command-line arguments
- Reads text files
- Searches for a given query
- Prints matching lines
- Uses `Config` for argument handling
- Separates application logic into `main.rs` and `lib.rs`
- Handles errors using `Result`

## Project Structure

```text
minigrep/
├── Cargo.toml
├── src/
│   ├── main.rs
│   └── lib.rs
└── poem.txt
```

## How to Run

Clone the repository:

```bash
git clone https://github.com/Prachi-Gupta2808/minigrep.git
cd minigrep
```

Build the project:

```bash
cargo build
```

Run the program:

```bash
cargo run -- <query> <file_path>
```

For example:

```bash
cargo run -- nobody poem.txt
```

## Example

Suppose `poem.txt` contains:

```text
I'm nobody! Who are you?
Are you nobody, too?
How dreary to be somebody!
```

Running:

```bash
cargo run -- nobody poem.txt
```

produces:

```text
I'm nobody! Who are you?
Are you nobody, too?
```

## Learning Goals

This project is part of my learning journey through **The Rust Programming Language Book**.

Through this project, I am learning:

- Command-line arguments
- Structs and methods
- `Result` and error handling
- Ownership and `clone`
- Modules
- Library and binary crates
- Testing
- File handling
- Iterators and string searching

## Technologies

- Rust
- Cargo

## Reference

Based on the `minigrep` project from:

[The Rust Programming Language](https://doc.rust-lang.org/book/ch12-00-an-io-project.html)

Based on the `minigrep` project from:

[The Rust Programming Language](https://doc.rust-lang.org/book/ch12-00-an-io-project.html)

# Functions

## Foreign function interface (FFI)

The **Foreign Function Interface** (FFI) is a mechanism that allows code written in one programming language to call functions or use libraries written in another language. It acts as a bridge, enabling seamless interaction between different languages, such as calling C functions from Python or Rust. FFI handles differences in data types, memory management, and calling conventions, making it essential for integrating diverse systems or leveraging existing libraries without rewriting code.

## Thrush solution

In Thrush, to call external code, we use the @extern("name") attribute, where the name represents the external function to be searched for at call time. This attribute only applies to functions; it is ignored by other structures.

```rust
fn sum(a: u64, b: u64) u64 @public @extern("sum_c");
```


# deref

This expression is used to dereference pointers or high-level pointers. It's a shortcut for loading values ​​from memory. It's similar to dereferencing a primitive type in Rust, and is used in other programming languages ​​with some kind of reference system. It's equivalent to ``*T`` in Rust.

This expression unwraps the type in one layer, loading the value from memory.

It is applicable for: 

- ``ptr[T]``
- ``ptr``
- ``mut T``

Where T is any type respecting the laws of the highest type.

## Code

```rust
fn main() u32 {
    local mutable_a: mut u32 = 0; 

    local not_mutable_a: u32 = deref mutable_a;

    return 0;
}
```
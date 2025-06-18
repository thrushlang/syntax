# Built-in 'sizeof'

## Information

The ``sizeof`` function is a built-in function that extracts the size of types at compile time and returns a numeric value at runtime. Its uses are exactly the same as ``sizeof()`` in **C**.

### Syntax

```rust
fn main() {

    local a: u32 = 10;

    local sizeof_a: u64 = sizeof(a);

}
```


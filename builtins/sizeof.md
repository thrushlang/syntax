# sizeof(T) u32

The ``sizeof`` function is a built-in function that extracts the size of types at compile time and returns a numeric value at runtime. Its uses are exactly the same as ``sizeof()`` in **C**.

## Types

- ``type`` **u32**
- ``args`` **T** (Any type, or reference)

### Code

```rust
fn main() {

    local a: u64 = 10;

    local sizeof_a: u32 = sizeof(a);

}
```


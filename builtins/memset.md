# Built-in 'memset'

## Information

The built-in function ``memset`` has the exact behavior of the one found in the standard C library. 

- For more information: __https://man7.org/linux/man-pages/man3/memset.3.html__

### Syntax

```rust
fn main() {

    instr a: ptr[u32] = alloc @stack { u32 };

    memset(a as ptr, 10, sizeof(u32));

}
```
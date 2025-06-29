# memset(ptr, u32 | u64, u32 | u64) void

The built-in function ``memset`` has the exact behavior of the one found in the standard C library. 

- For more information: __https://man7.org/linux/man-pages/man3/memset.3.html__

## Types

- ``type`` **void**
- ``args`` **ptr**, **u32** | **u64**, **u32** | **u64**

### Code

```rust
fn main() u32 {

    instr a: ptr[u32] = alloc @stack { u32 };

    memset(a as ptr, 10, sizeof(u32));

    return 0;

}
```

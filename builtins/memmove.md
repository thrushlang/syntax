# memmove(ptr, ptr, u32 | u64) ptr

The built-in function ``memmove`` has the exact behavior of the one found in the standard C library. 

- For more information: __https://www.man7.org/linux/man-pages/man3/memmove.3p.html__

## Types

- ``type`` **ptr**
- ``args`` **ptr**, **ptr**, **u32** | **u64**

### Code

```rust
fn main() u32 {

    instr a: ptr[u32] = alloc @stack { u32 };
    instr b: ptr[u32] = alloc @stack { u32 };

    memmove(b as ptr, a as ptr, sizeof(u32));

    return 0;

}
```

# memcpy(ptr, ptr, u64) ptr

The built-in function ``memcpy`` has the exact behavior of the one found in the standard C library. 

- For more information: __https://man7.org/linux/man-pages/man3/memcpy.3.html__

- ``type`` **ptr**
- ``args`` **ptr**, **ptr**, **u64**

### Code

```rust
fn main() {

    instr a: ptr[u32] = alloc @stack { u32 };
    instr b: ptr[u32] = alloc @stack { u32 };

    memcpy(b as ptr, a as ptr, sizeof(u32));

}
```

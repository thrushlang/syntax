# alignof(T) u32

The built-in ``alignof`` function extracts the memory alignment of a specific type at compile time. It is deterministic, corresponding to the architecture and type.

## Types

- ``type`` **u32**
- ``args`` **T** (Any type, or reference)

### Syntax

```rust
fn main() u32 {

   local memory_align: u32 = alignof(u8);

   return 0;

}
```

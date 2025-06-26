# alignof(T) u32

The built-in ``alignof`` function extracts the memory alignment of a specific type at compile time. It is deterministic, corresponding to the architecture and type.

- ``type`` **u32**
- ``args`` **T** (Any type, or reference)

### Syntax

```rust
fn main() {

   local memory_align: u32 = alignof(u8);

}
```

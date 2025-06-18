# Casts

## General Information

Casting allows you to transform any type at compile time. It's useful for converting them to direct pointers.
This is equivalent to ``as`` keyword in rust, it is evaluated at compile time and determined if possible.

```rust
fn main() {

    local a: u32 = 100;

    instr b: ptr[u32] = a as ptr[u32];
    
    write b, u32 1000; // a = 1000;

}
```
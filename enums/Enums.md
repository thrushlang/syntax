# Enums

## General Information

In thrush enums allow you to have constants as variants of enums, in addition to dynamic values.

```rust
enum Colors {
    Red: u32 = 0;
    Yellow: u32 = 1;
    Blue: u32 = 2;
}

// Compile time function.
fn jit_test() u32 @comptime {
    return 1231 / 1231;
}

enum DynamicColors {
    Red: u32 = jit_test(); // In the future this will be allowed, but not until the Just-In-Time Compiler (JIT) is finished.
}

fn main() {
    local yellow_plus_red: u32 = Colors->Yellow + Colors->Red;
}
```

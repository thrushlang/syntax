# Functions

```rust
// Syntax: <linkage-qualifier> fn <name> () : <type> ; | { ... }

// Complete function definition
fn my_function(): void {}
```

```rust
// External function declaration (FFI) (C convention)
public @extern("malloc") fn alloc(size :: i32): ptr;
```

```rust
public fn my_function(): void {}

fn main() {
    // Function call
    my_function()
}
```

```rust
public fn my_function(): i64 {
    // Function return
    return 10;
}

fn main() {
    var some_function_value: i64 = my_function(); 
}
```
# Conditionals

```rust 
fn main() {

    // NOTE: Non-chained conditions aren't allowed, as Rust.

    var allowed: bool = 123 == 122;

    if allowed {
        ...
    } elif allowed == false && 12 == 12 {
        ...
    } else {
        ...
    }

}
```
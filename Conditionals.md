# Conditionals

Unchained conditionals are not allowed in Rust for reasons of unnecessary complexity in the compiler. Values ​​like this `123 == 123 == 123` are not allowed; instead, it should be `123 == 123 && 123 == 123`.

```rust 
fn main() {

    // NOTE: Unchained conditions aren't allowed, as Rust.

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
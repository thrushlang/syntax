# Variables

```rust
fn main() {
    // Syntax: <linkage-qualifier> var <name>: <type> ; | = <value>; 

    // Always mutable, complete variable definition.
    var my_first_var: i64 = 0;

    // Variable mutation.
    my_first_var = 123;

    // Variable definition without value.
    var my_second_var: bool;

    // Variable mutation.
    my_second_var = true;

    // Variable with public linkage. It's only allowed inside the classes.
    public var my_first_var: i64 = 0;
}
```
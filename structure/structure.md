# Structures

Structures behave like in languages ​​like C. They are traditional structures.

## Memory Information

- Allocation site: ``Stack or Heap``.
- Prefer allocation site: ``Stack``.

## Code

```rust
struct MyStruct {
    size: s64
    length: s32
    matter: bool
}
```

```rust
struct MyStruct {
    size i64
    length i32
    matter bool
};

fn main() {
    local some_struct: MyStruct = MyStruct {
        matter: true,
        length: 12,
        size: 12312
    };
}
```


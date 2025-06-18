# Structures

## Memory Information

- Allocation site: ``Stack or Heap``.
- Prefer allocation site: ``Stack``.
- Is it released automatically?: ``Yes``.

## Information

Structures are automatically deallocated from memory when they reach the EFC (End of the Function Context), functioning as destructors embedded in the language.

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
    local some_struct: MyStruct = new MyStruct {
        matter: true,
        length: 12,
        size: 12312
    };
}
```


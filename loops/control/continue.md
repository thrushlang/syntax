# Continue | Loop Control Flow

It behaves exactly the same as in C, it continues to the next iteration.

## Code

```rust
for local mut i: u32 = 0; i < 1000; ++i; {
    if i >= 666 {
        continue;
    }
}
```
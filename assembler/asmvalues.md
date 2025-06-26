## Assembler Values

Assembler values ​​are blocks of code made entirely in assembler that can be used as common values ​​in the language.

## Code

```rust
fn main() {

    local whatever: u32 = asm u32 {
        "mov $$42, %eax"
    } {
        ""
    } + 20;

}
```

## LLVM Inline Assembler

The syntax depends on each backend usage. If you use the LLVM backend with ``-llvm``, the syntax within the assembler will be the one supported by LLVM by default. For more information, see: https://llvm.org/docs/LangRef.html

<img src= "https://github.com/thrushlang/syntax/blob/master/assets/LLVM-inline-assembler-ref.png" alt= "llvm-inline-assembler-ref" style= "width: 50%; height: 50%;"> </img>
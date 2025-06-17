# Assembler Functions

## General Information

Assembler functions are purely assembler-based functions. They support Intel & AT&T x86_64 assembler.

```rust
asmfn invoke_exit_syscall() void {
    "mov $$60, %rax",
    "mov $$1, %rdi",
    "syscall" // Assembler Code
} { 
    "~{rax}~{rdi}" // Constraints
}

fn main() {

  invoke_exit_syscall();

}
```

## LLVM Inline Assembler

The syntax depends on each backend usage. If you use the LLVM backend with ``-llvm``, the syntax within the assembler will be the one supported by LLVM by default. For more information, see: https://llvm.org/docs/LangRef.html

<img src= "https://github.com/thrushlang/syntax/blob/master/assets/LLVM-inline-assembler-ref.png" alt= "llvm-inline-assembler-ref" style= "width: 50%; height: 50%;"> </img>
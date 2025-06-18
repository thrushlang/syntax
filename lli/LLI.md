# Low Level Instruction

## Information

Low-level instructions are a high-level version of IR, allowing the programmer to modify the compiler's code generation to their liking. In addition to serving as a bridge to the assembler abstraction, they allow the language to delve much deeper into the hardware. Currently, neither C, C++, nor Rust allow explicit modification of low-level instructions from source code.

### ALLOC (LLI)

Allows you to allocate a memory space in any location.

Valid site allocations:

- ``@stack``
- ``@heap``
- ``@static``

```rust
instr new_value_allocated: ptr[u8] = alloc @stack, { u8 };
```

### WRITE (LLI)

Allows you to overwrite a value in memory.

```rust
write new_value_allocated, u8 8;
```

### LOAD (LLI)

Allows you to load any value from memory.

```rust
instr value: u8 = load u8, new_value_allocated;
```


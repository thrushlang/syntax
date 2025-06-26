# Primitives types

Primitive types are types built into the language, basic and essential.

## Integer Types

### Unsigned integer types

- ``u64`` unsigned integer 64 bits.
- ``u32`` unsigned integer 32 bits.
- ``u16`` unsigned integer 16 bits.
- ``u8`` unsigned integer 8 bits.

### Signed integer types

- ``s64`` signed integer 64 bits.
- ``s32`` signed integer 32 bits.
- ``s16`` signed integer 16 bits.
- ``s8`` signed integer 8 bits.

## Floating-Point Types

- ``f32`` Floating-Point Type 32 bits (IEEE 754, single precision)
- ``f64`` Floating-Point Type 64 bits (IEEE 754, double precision)

## Boolean type

- ``bool`` Boolean logical type.

## Fixed Array type

- ``fixed[T; N]`` Type with a size that is known at compile time.

## Array Type

- ``[T]`` Type with a size that is known at runtime.

## Pointer Type

- ``ptr[T]`` C-style pointers, but strongly typed.

## High Level Pointer Type

High-level pointers are named for a class of characteristics that require the use of memory-safe patterns when using this specific type. Some of their characteristics are:

- They are only one depth.
- Avoid memory aliasing at all costs.
- Pointer types are not supported. Only values.

### Code

- ``mut T``
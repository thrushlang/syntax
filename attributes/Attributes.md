# Attributes

## General Information

Attributes allow you to modify code generation, code execution, visibility, 
call conventions, memory management, and much more. They are direct code modifiers.

### Visibility

- ``@public`` Modifies the visibility of the structure to which it is attached.

### Call Conventions

Calling conventions define how functions pass arguments, return values, and manage the stack during function calls.

### Supported Call Conventions

- ``C`` = The C call convention.
- ``fast`` = Optimized for speed, passes arguments in registers and minimizes stack usage.
- ``tail`` = Enables tail-call optimization, reusing the stack frame for efficient recursive calls.
- ``cold`` = For rarely called functions, prioritizes smaller code size over execution speed.
- ``weakReg`` Preserves most caller-saved registers, balancing performance and compatibility.
- ``strongReg`` Preserves all caller-saved registers, ensuring maximum compatibility but with higher overhead.
- ``haskell`` = Glasgow Haskell Compiler (GHC) 
- ``erlang`` = High-Performance Erlang Compiler (HiPE).
- ``swift`` = Swift

#### Example:

- ``@convention("haskell")``

## Optimizations

The attributes from @hot onward guide the compiler to optimize functions by balancing performance, code size, security, and precision, either by prioritizing speed (e.g., inlining, frequent execution), minimizing code size, enhancing memory safety with stack protections, or ensuring accurate floating-point operations, depending on the specific attribute applied.

- ``@hot`` = Marks a function as frequently executed, prioritizing optimizations for performance.
- ``@noinline`` = Prevents the function from being inlined, ensuring it remains a separate call.
- ``@inlinehint`` = Suggests the function should be inlined for performance, but not cmandatory.
- ``@minsize`` = Optimizes the function for minimal code size over speed or other factors.
- ``@alwaysinline`` = Forces the function to be inlined at all call sites, regardless of cost.
- ``@safestack`` = Uses a separate stack for sensitive data, enhancing memory safety.
- ``@strongstack`` = Enforces strict stack-smashing protection.
- ``@weakstack`` = Applies minimal stack protection, trading security for performance.
- ``@precisefp`` = Ensures precise floating-point operations, avoiding aggressive optimizations that alter results.

## Unique attributes

`@comptime` This attribute allows code execution at compile time, through a Just In Time Compiler (JIT).
# Structures

```rust
// Struct definition

public struct MyStruct {
    size i64
    length i32
    matter bool
};
```

```rust
// Struct native construction

public struct MyStruct {
    size i64
    length i32
    matter bool
};

fn main() {

    var some_struct: MyStruct = new MyStruct {
        matter true
        length 12
        size 12312
    };

}

```

```rust
// Struct methods

public struct MyStruct {
    size i64 // Always public field
    length i32 
    matter bool
};

for MyStruct {

    // Struct constructor
    fn new(): self {
        pass
    }

    // Public method
    public fn dealloc(): void {
        @internal dealloc(this);
    }

    // Private method
    fn set_size(new_size :: i64): void {
        this.size = new_size;
    }
}

```

```rust
// Struct method access 

public struct MyStruct {
    size i64 // Always public field
    length i32 
};

for MyStruct {

    // Struct constructor
    fn new(): self {
        pass
    }

    // Public method
    public fn dealloc(): void {
        @internal dealloc(this);
    }

    // Public method
    public fn set_length_and_size(length :: i64, size :: i64): void {
        this.set_size(size);
        this.length = length;
    }

    // Private method
    fn set_size(new_size :: i64): void {
        this.size = new_size;
    }
}

fn main() {

    var some_struct: MyStruct = MyStruct.new();

    some_struct.set_length_and_size(0, 0);
    some_struct.dealloc();
}
```


## General Information

Methods in thrush are called ``bindings``, they allow you to create methods for a type of structure.

```rust
struct MyStruct {
    size: s64
    length: s32
    matter: bool
}

bindings MyStruct {
    bind new() MyStruct {
        local my_structure = new MyStruct {
            size: 0,
            length: 0,
            matter: false
        };

        return my_structure;
    }

    bind set_size(this mut, new_size: s64) void {
        this.size = new_size;
    }

    bind set_length(this mut, new_length: s32) void {
        this.length = new_length;
    }

    bind set_matter(this mut, new_matter: bool) void {
        this.matter = new_matter;
    }
}

fn main() {

    local mut my_struct: MyStruct = MyStruct::new();

    my_struct.set_size(10);
    my_struct.set_length(100);
    my_struct.set_matter(true);

}

```
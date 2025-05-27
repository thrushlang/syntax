## General Information

Methods in thrush are called ``methods`` literally, they allow you to create methods for a type of structure.

```rust
struct MyStruct {
    size: s64
    length: s32
    matter: bool
}

methods MyStruct {
    fn new() MyStruct {
        local my_structure = new MyStruct {
            size: 0,
            length: 0,
            matter: false
        };

        return my_structure;
    }

    fn set_size(this mut, new_size: s64) void {
        this.size = new_size;
    }

    fn set_length(this mut, new_length: s32) void {
        this.length = new_length;
    }

    fn set_matter(this mut, new_matter: bool) void {
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

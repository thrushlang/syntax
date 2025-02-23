# Classes

```swift
public class MyClass {

    // Properties definition
    public var first_property: i64 = 0; 
    public var second_property: bool = 0; 

    // Multiple arguments are allowed.
    fn init(arg_one :: i64, arg_two :: bool): void {
        // Constructor method. Always needed for the compiler.
        ...

        this.second_property = arg_two;
    }

    public fn some_method(): void {
        this.first_property =  123;
    }
}   

fn main() {

    var some_class: MyClass = MyClass.init(0, false);

}
```
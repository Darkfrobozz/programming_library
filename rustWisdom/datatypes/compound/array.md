Arrays have a uniform type.
Moreover, they have a fixed length.
Standard bracket notation is used for access.
Initialization can be done through
```rust
let a: [i32; 5] = [1, 2, 3, 4, 5];
```
The important part to notice here is the first bracket pair, this specifies how long the array is and what type. (Not necessary in this case).

You can also use this notation to fill all the elements:
```rust
let a = [3; 5];
```
## Invalid Access
This results in a [[panic]].
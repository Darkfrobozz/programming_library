Tuples can be constructed with a fixed length through:
```rust
let tup = (500, 6.4, 1);
```
But interestingly, they can also be respectively deconstructed like this:
```rust
let (x, y, z) = tup;
```
We can also access the elements directly by, starting from 0, do:
tup.0 // = 500
tup.1 // = 6.4
tup.2 // = 1
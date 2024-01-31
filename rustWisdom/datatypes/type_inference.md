Using our Rust [[type_system]], we are able to determine types without the user explicitly saying which type it is.

However, when multiple types are possible, we have to specify the type to be used.
```rust
let guess: u32 = "42".parse().expect("Not a number!");
```

Without u32 here we will get a compiler error demanding type annotations.
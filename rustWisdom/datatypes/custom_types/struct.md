This develops further on the idea of [[named_tuple]]s. 
In this, we have not only custom names but also custom indexes.
They are in a way static structured [[tuple]]s. Less flexible during runtime but more specific.

This is how we introduce a struct :
```rust
struct User {
    active: bool,
    username: String,
}
```

To access members of this structured pair we use dot notation.

We can also leave out all the fields to get an empty [[struct]], this can be used for traits.

We need a [[data_lifetime]] to store references in our structs. Without that, we need to make all the data owned by that struct.
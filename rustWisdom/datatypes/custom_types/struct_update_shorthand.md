When defining a new instance of a [[struct]] based on a previous instance we can use a shorthand :
```rust
fn main() {
    // --snip--

    let user2 = User {
        email: String::from("another@example.com"),
        ..user1
    };
}
```
Here the *..user1* tells us to fill the remaining fields with corresponding information from that instance.
We can store more information in our [[enum]] by when declaring them adding a [[tuple]] portion containing data associated with the [[enum]]:
```rust
enum IpAddr {
	V4(String),
	V6(String),
}

let home = IpAddr::V4(String::from("127.0.0.1"));

let loopback = IpAddr::V6(String::from("::1"));
```

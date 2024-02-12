Sometimes we only want to disclose a segment of some data then we send a pointer to that segment.
## The Problem
Think of the problem of throwing around indexes tied to some array.
The computer has no idea that these indexes don't mean what they did before when we remove the array.
Therefore, what we want is not an index but rather a link to the array.

## The Solution
The solution that was arrived as what slices, the following notation is used for that :
```rust
	let mut s = String::from("hello world");
	let hello = &s[0..5];
```

## Literals
These are in fact slice of the binary.

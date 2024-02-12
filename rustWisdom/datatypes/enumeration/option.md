There is an [[enum]] used by the standard library that is called option.
This is especially relevant when considering return values from functions.
There are situations when we want to know whether the [[function_call]] failed or not.

A common variant of data is whether there is or is not data.
The way [[enum]] solves this is that it makes handling these two situations mutually exclusive.
You will know exactly when you are handling the *null* result and when you are handling real data.

This choice is important because it helps protecting systems from human error.

```rust
enum Option<T> {
    None,
    Some(T),
}
```

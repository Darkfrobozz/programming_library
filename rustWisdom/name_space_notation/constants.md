These are always immutable.

They may only be calculated at build time, this implies that they are not only immutable but also static.

These constants can however be calculated by the compiler and there are certain operations that are allowed when specifying a constant.

Here is an example program:
```rust
const THREE_HOURS_IN_SECONDS : u32 = 60 * 60 * 3;
```

These properties lends itself to values that are hardcoded.

Rust uses the name references to describe pointer like variables that point to a specific place where a pointer to value is stored.

This means that the original value is not dropped when the reference is.

A reference's scope starts where it is defined and ends when it is used last.

A reference cannot live past its owner and the compiler actively prevents us from creating references that will.
This is to prevent access to memory that have been dropped.
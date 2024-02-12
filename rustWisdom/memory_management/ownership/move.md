By [[ownership]] there is at most one owner at a time.

Think about a [[string]] :

When we copy that string into a new variable, what we are actually copying is only the [[struct]] that is on the [[stack_mem]] not the part that is in [[heap_mem]].
```rust
    let s = String::from("hello");
    println!("{s}");
    let s2 = s;
```
We now, since we did not copy the heap memory, have a new owner for that heap memory.
Consequently, $s$ is no longer valid. In fact calling on it will result in a compile time error.

This copying of the [[struct]] on [[stack_mem]] is thus called a [[move]].
Essentially, we have moved the ownership of the [[heap_mem]] segment.

This part about the changing the owner of the string also applies to sending the string as an argument to a [[function_call]].
Moreover, it also moves ownership with the return of a [[function_call]].
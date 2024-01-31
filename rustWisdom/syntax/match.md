The match is a super powerful expression of pattern matching.
```rust
    match guess.cmp(&secret_number) {
        Ordering::Less => println!("Too small!"),
        Ordering::Greater => println!("Too big!"),
        Ordering::Equal => println!("You win!"),
    }
```
Each *Ordering* part here is a possible outcome and the compiler, being our friend, reminds us to match all the outcomes.

match can also be used instead of [[expect]] to handle [[result_variants]] more effectively rather than just crashing.
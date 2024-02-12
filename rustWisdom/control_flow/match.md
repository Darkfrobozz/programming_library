The match is a super powerful expression of pattern matching.

Moreover, its pattern matching is exhaustive.
# Analogy
There is a quite fitting analogy to the match machine, it is like a coin sorting slide.
Imagine letting multiple coins slide in and then having different gaps in increasing order, then the different coins will fall into the correct gap, the first gap big enough.
# Example
```rust
    match guess.cmp(&secret_number) {
        Ordering::Less => println!("Too small!"),
        Ordering::Greater => println!("Too big!"),
        Ordering::Equal => println!("You win!"),
    }
```
The [[enum]] *Ordering* has three possible outcome and the compiler, being our friend, reminds us to match all the outcomes to some [[arm]].

match can also be used instead of [[expect]] to handle [[result_variants]] more effectively rather than just crashing.

# Variable Binding
We can also use match [[arm]]s as lambda functions in the sense that we can extract components from the [[enum]]s.
# Special Patterns
- other : Default case
- _ : Garbage default case
- _ =>() : Garbage do nothing
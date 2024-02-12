A problem with [[move]] is that sometimes we want a copy with strings we can call *clone*:

```rust
    let s1 = String::from("hello");
    let s2 = s1.clone();

    println!("s1 = {}, s2 = {}", s1, s2);
```

However, what about this, shouldn't this be [[move]] and violate [[ownership]].
But both of these variables sizes are known at compile time. 
Thus, their copy methods are constant and relatively inexpensive. 
Consequently, they are annotated with the *Copy* trait which says that the variable can be copied on like this :
```rust
    let x = 5;
    let y = x;

    println!("x = {}, y = {}", x, y);
```
However, if some structure is annotated with *Copy* but implements [[drop]], then, the compiler will be angry.
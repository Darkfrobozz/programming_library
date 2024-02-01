## How to Start the Loop
This is the most basic way of repeating code in Rust.
It contains a scope and repeats forever until we explicitly tell it within the scope to stop.
```rust
    loop {
        println!("Please input your guess.");

        // --snip--

        match guess.cmp(&secret_number) {
            Ordering::Less => println!("Too small!"),
            Ordering::Greater => println!("Too big!"),
            Ordering::Equal => println!("You win!"),
        }
    }
```

## How to Control It
There are two keywords that we need to use for effective control of the loop:
- break : 
	- Hops out of the loop
	- Can be modified with a value to return => needs ; at the end since it is now an expression
- continue - Ends the current iteration 

## Labeling
A loop label must start with "'".
This is for the computer to know which loop you are referring to when you try to control the loop.
```rust
    let mut count = 0;
    'counting_up: loop {
        println!("count = {count}");
        let mut remaining = 10;

        loop {
            println!("remaining = {remaining}");
            if remaining == 9 {
                break;
            }
            if count == 2 {
                break 'counting_up;
            }
            remaining -= 1;
        }

        count += 1;
    }
```
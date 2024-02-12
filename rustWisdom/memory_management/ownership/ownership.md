## Theory
The basic wish is utilize memory efficiently to do that rust uses a unique concept called ownership.

There are three rules:
- Each value in Rust has an owner.
- There can only be one owner at a time.
- When the owner goes out of [[scope]], the value will be [[drop]]ped.
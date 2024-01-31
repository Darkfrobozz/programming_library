## Annotation
Integers in rust can be represented with:
{u32, i16, usize ... }

These parts mean:

u -> unsigned, i -> signed

num -> bytes : range 8, 16 ... 128 OR:
	size -> Platform dependent.
## Overflow
When using a too large integer in a too small integer storage, integer overflow occurs.
These result in two different cases:
- debug: [[panic]].
- release: wrap around.
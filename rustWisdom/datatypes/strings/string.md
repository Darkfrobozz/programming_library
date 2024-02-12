To initialize an empty string with no memory, we use [[UTF-8]] encoding, this enables variable width encoding.
This also means that strictly, strings are not arrays of [[character]]s but truncated [[character]]s.
	*String::new*

A string consists of three parts in a struct:
- Pointer -> memory of chars on the heap
- Length
- Capacity
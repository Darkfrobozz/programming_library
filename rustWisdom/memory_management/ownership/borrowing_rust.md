The act of creating a [[reference_rust]] is the act of borrowing similar to real life when we borrow something we do not acquire [[ownership]].

To create a [[reference_rust]] we use *&* operator on a [[name_spaces]].
This is by default immutable, meaning we can not write through this borrow only read.

We can augment this borrow to be mutable but that leads to us not being able to have any other borrows.

The reason for this is to prevent [[data_race]].
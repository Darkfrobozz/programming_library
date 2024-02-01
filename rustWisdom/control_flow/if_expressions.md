## Main Idea

These are [[expression]], which means that they are joined by more code, in this case, [[arm]]s.

Think of the [[arm]]s as not being used if the 'if_expression' evaluates to false.

It is important to note that if expressions take bool arguments.

## Supplementing with Else

If the expression evaluates to false it may be interesting to note what the code does in that case.
To control that we can use 'else' or 'else if'.

## Utilizing Expression Part 

Since these are [[expression]]s, we have that if some [[arm]] does not end itself with ';', it does not turn into a [[statement]].

Thus, the whole if statement can be used as an expression in more code.

But then the different [[arm]]s must have types that make sense in the context of the presence of the code using it.
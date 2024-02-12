These types of functions are a generalization of [[method]], they extend to all [[function_signature]] that can be in an *impl* block.

For example, a [[function_signature]] that does not take as parameter &self is not a [[method]] but it nonetheless an associated function.

To preform a [[function_call]] on such a function we must use *::* notation.
This way we can access all the function defined by the struct namespace.

We may also define multiple *impl* blocks for the same [[struct]].
At its core a method is a [[function_signature]] that is defined in the context of some struct.
Their first parameter is always *self*, which refers to the instance that initiated the [[function_call]].
This is an interesting aspect, as it makes it so that the function is not in the environment of the struct but rather creates a short hand to elucidate that it is for passing the environment to the function.

To access these we use dot notation and to tie a [[function_signature]] to a struct and create our method we use an *impl* (implementation) block.

Moreover, our method allow for [[variable_shadowing]] since we can discern if it is a [[function_call]] or a property access based on context.
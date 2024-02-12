In rust we often as developers want to see what our [[struct]]s are like at some point in the program.
Therefore, it is very convenient to use the debug trait which allows for various way to print to the user different structs.
For example *{:?}* is for simply printing on the line the information available on the struct and *{:#?}* formats so that it is on multiple lines.

Moreover, we can also use the *dbg!* macro to print debugging information about some expression to our std_err.
Thus, we can use this for logging.

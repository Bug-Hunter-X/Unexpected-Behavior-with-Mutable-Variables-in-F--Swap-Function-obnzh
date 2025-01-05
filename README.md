# F# Mutable Variable Swap Bug

This example demonstrates a common error when working with mutable variables in F#.  Because F# passes mutable variables by reference, a seemingly simple swap function can produce unexpected results if you are not aware of this subtle behavior.

The `bug.fs` file contains the buggy code, while `bugSolution.fs` shows the corrected version.  The core issue is that the swap function directly modifies the original `x` and `y` variables, instead of returning new values.
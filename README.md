# Lua `pairs` Iteration Order Issue in Recursive Function

This repository demonstrates a potential issue with Lua's `pairs` iterator when used in recursive functions.  The `pairs` iterator does not guarantee a specific iteration order, which can lead to unpredictable results, especially when dealing with nested tables with non-integer keys.

The `bug.lua` file shows a simple recursive function that iterates through a nested table using `pairs`. The order of processing the nested tables is not defined, which could cause unexpected outcomes depending on the Lua implementation and the table's structure.  

The `bugSolution.lua` provides a solution using a different method for table traversal that ensures predictable iteration order.
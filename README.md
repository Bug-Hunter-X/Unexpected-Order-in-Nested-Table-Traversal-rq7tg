# Lua Nested Table Traversal Bug

This repository demonstrates a subtle bug related to the order of iteration in nested Lua tables using the `pairs` iterator.  The `pairs` function does not guarantee any specific order of iteration, which can lead to unexpected results when processing nested tables recursively, as shown in the `bug.lua` file.

The solution in `bugSolution.lua` shows a way to address this by using an explicit sorting mechanism or a different traversal approach, which guarantees deterministic behavior. 

## Setup

To reproduce the issue, simply run the `bug.lua` script. The `bugSolution.lua` contains the fix.
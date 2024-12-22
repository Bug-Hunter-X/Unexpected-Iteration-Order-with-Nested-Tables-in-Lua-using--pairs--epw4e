# Lua Nested Table Iteration Issue

This repository demonstrates a potential issue with Lua's `pairs` iterator when working with deeply nested tables.  The `pairs` function does not guarantee a specific iteration order, which can lead to unexpected results in recursive functions that depend on a consistent order.

The `bug.lua` file contains a simple example of a recursive function that iterates over a nested table. The output may vary depending on the Lua interpreter. The `bugSolution.lua` file demonstrates a solution using a more predictable iteration method.
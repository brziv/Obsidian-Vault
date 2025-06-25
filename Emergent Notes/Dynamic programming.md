#theory

A method of solving problems by breaking them into smaller, easier sub-problems. It is very related to iteration and recursion.

Bottom-up:
	Solve small sub-problems
	Store solutions
	Reuse results for larger sub-problems
	-> construct a table

Top-down:
	Break to smaller problems
	Stop at base cases
	Solving upward, caching results
	-> recursion using a stack

In theory, they are equally efficient, but in practice, bottom-up is preferred:
	Stack overhead, overflow
	CPU cache (memory)
	Compiler optimization
	The nature of problems (sub-problems are necessary)

[[Rod cutting]]

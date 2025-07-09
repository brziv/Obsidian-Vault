#theory 

A method of finding the convex hull of a set of points.
	Find the first point (lowest y then x)
	Sort other points by polar angle
	Set up a stack with first 2 points
		If right turn (current and top 2), pop top 1
		Push current into stack
	Stack contains the convex hull
str8ts solver with constraint programming
======
written in SWI-Prolog using the clpfd library

more about str8ts puzzles and their rules at [http://www.str8ts.com/](http://www.str8ts.com/)

usage
-----
	Puzzle = [[1,2,3,4,5,6,7,_,"b"],
	          [2,3,4,5,_,7,8,9,"b"],
	          [3,_,"b",6,7,_,"b","b","b"],
	          [_,5,6,7,8,"b",1,_,"b"],
	          [5,6,7,8,9,1,2,3,4],
	          [_,7,8,_,"b",2,_,4,5],
	          [7,_,"b",1,2,_,4,"b",_],
	          [_,9,"b",2,3,4,_,6,7],
	          ["b",1,_,3,4,"b5",6,_,8]], str8ts(Puzzle).


known issues
--------
- depending on the puzzle more than ~25 empty cells will result in very long computation times with an exponential increase with each additional empty cell

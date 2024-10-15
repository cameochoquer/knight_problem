# GUIDELINES:
1. Everyone should contribute
2. AI tools allowed for research but please don't copy & paste code
3. Act as if you were a team of equals solving a problem in
 a staging enviroment that would go to production
(minus tests & git).
4. This is an assessment of communication not completeness
or finding the solution


# PROBLEM:
In the game of chess you have an 8x8 board, in this puzzle you
are given one piece, the knight. The Knight moves in a L shape,
2 spaces vertically or horizontally and then 1 space in the
perpendicular direction.

# Visual representation:
- https://files.herculeschess.com/file/herculeschess/2023/02/Knight-Movement-1024x1024.png

In this puzzle you have been given a modified board (see below).
This board is marked with empty spaces (0s) and blocked spaces (1s)
your knight cannot enter a blocked space at any point.

You also have a list of co-ordinate pairs, for each pair of
co-ordinates find the shortest route between the 1st and 2nd
co-ordinate. I.e. for the pair (0,0) -> (1, 2) the answer would be 1.
If a route isn't possible, where the final space is blocked or
with the existing blocks there is no possible route, return -1.

# EXTENSION:
The Knight's problem is generally solved in O(2) time.
However it is possible in O(1) with contstraints, try it.

# Test routes/example start and end positions
# (0,2) -> (0,7)
# (2,6) -> (1, 2)
# (7, 1) -> (7, 2)
# (5,3) -> (2, 7)
# (6,4) -> (4,3)
# (6,2) -> (4,3)
# (0, 7) -> (0,6)

board = [
    [0, 0, 0, 0, 1, 0, 0, 0],
    [1, 0, 0, 0, 0, 1, 0, 0],
    [0, 0, 0, 0, 0, 0, 0, 0],
    [0, 0, 0, 0, 0, 1, 0, 0],
    [1, 0, 0, 1, 0, 0, 0, 0],
    [0, 1, 0, 0, 0, 0, 0, 0],
    [0, 0, 1, 0, 0, 0, 0, 0],
    [0, 0, 0, 0, 0, 0, 1, 0],
]
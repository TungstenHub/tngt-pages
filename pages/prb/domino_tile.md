Can we tile a $10\times 10$ board with the top left and right bottom squares removed with $2\times 1$ dominoes? If not, why?

{{ image | domino_tile }}

+++
Solution
+++

This problem is a very tricky and interesting one. No matter how easy it seems, after a few tries one may suspect that no tiling fits the described board - there are always at least two empty squares. Indeed, it is not possible to tile such board with dominoes. But how can we prove it? Checking all combinations is simply not possible

There is a remarkably simple and effective argument: paint the board in black and white, as a chessboard. Each domino tile has to cover a black square and a white square. We will always cover the same number of black and white squares. But the removed squares where of the same color, so _our board has a different number of black and white squares_. And then we can't tile our board

{{ image | domino_tile_chess }}

+++
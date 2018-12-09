Chess on a Website
----

Website link: http://chess99901.atwebpages.com/

A very simple Chess AI.

The following chess programming techniques are used:
1) Move generation
2) Board Evaluation
3) Minimax
4) Alpha Beta Pruning

Step - 1 : Move Generation
---

The chess.js is used for move generation, whereas the chessboard.js library is used for the design of the chessboard. The move generation library basically implements all the rules of chess. Based on this, all legal moves for a given board state are calculated. Other than the libraries used for move generation and board visualization, the core javascript code focuses on using the algorithm that finds the best move. This step just return a random move from all of the possible moves. 

Step - 2 Evaluation of position
---

To evaluate which side is stronger in a certain position, the relative strength of the pieces on the board is counted. The evaluation function chooses the move that gives the highest evaluation.

Step - 3 Minimax
---

Using the Minimax algorithm, the best move is chosen from a search tree. In this algorithm, the recursive tree of all possible moves is explored to a given depth, and the position is evaluated at the ending “leaves” of the tree.
After that, we return either the smallest or the largest value of the child to the parent node, depending on whether it’s a white or black to move. (That is, we try to either minimize or maximize the outcome at each level.)

Step - 4 Alpha Beta Pruning
---

Some branches in the search tree are disregarded by applying Alpha-beta pruning to the Minimax algorithm. It is based on the situation where we can stop evaluating a part of the search tree if we find a move that leads to a worse situation than a previously discovered move. The alpha-beta pruning does not influence the outcome of the minimax algorithm — it only makes it faster.

Bonus - Improved version
---

As an improvement, a factor that takes in account the position of the pieces is added to the evaluation. 

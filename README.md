# Tic-Tac-Toe AI Game

In the realm of classic entertainment, I've brought the universally enjoyed game of Tic-Tac-Toe to life through the Python implementation featuring a user-friendly graphical interface powered by the PyGame library. Players can relish the timeless 'X' versus 'O' match-up, with the added thrill of challenging an AI opponent at varying difficulty levels: Easy, Medium, or Hard.

## AI Algorithm

At the core of our game lies the sophisticated Minimax algorithm, a strategic decision-making process widely recognized in the domain of two-player turn-based games. This algorithm, accompanied by a scoring system of 1 for the maximizer, -1 for the minimizer, and 0 for a draw, ensures that the AI player optimally chooses its moves by recursively exploring possibilities and selecting the most advantageous move at each turn.

## Optimizations

To enhance the efficiency of our AI, we've integrated several key optimizations:

1. **Alpha-Beta Pruning**: 
    - We've incorporated a dispatch function calling the `max_value` and `min_value` functions selectively.
    - This powerful optimization technique significantly reduces the number of nodes evaluated in the search tree, contributing to a more responsive and formidable AI opponent.

2. **Depth-Limited Search Strategies**: 
    - By imposing a cap on the number of moves the AI considers ahead, we strike a balance between computational efficiency and strategic exploration.
    - I start from a depth of 0 and increment by 1 for each recursive call until we reach a maximum depth of 5, at which the AI performs its evaluation.
    - Additionally, I've modified the utility function in the depth-limited search to prioritize faster victories and losses.

## Difficulty Levels

- **Easy**: 
    - The AI opponent opts for random moves, providing an accessible and less strategic gaming experience.
- **Medium**: 
    - The AI's decision-making is elevated, employing the Minimax algorithm with Alpha-Beta pruning to determine optimal moves, ensuring a more competitive and challenging match for players.
- **Hard**: 
    - This level introduces a more sophisticated approach by incorporating depth-limited Minimax with Alpha-Beta pruning.

## How to Run the Code

To run the Tic-Tac-Toe AI game on your local machine, follow these steps:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/Mariamhsein2001/TicTacToe.git
    ```
2. **Install the required dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Run the game**:
    ```bash
    python TicTacToe.py
    ```

This will launch the game window, allowing you to play Tic-Tac-Toe against the AI opponent.

## Conclusion

The implementation of the classic game Tic-Tac-Toe represents a harmonious blend of user-friendly design and advanced artificial intelligence. 

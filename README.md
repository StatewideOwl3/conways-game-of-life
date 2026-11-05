# Conway's Game of Life
This is my toy implementation of Conway's game of life using python and pygame.
To run, clone the repo, create a python virtual environment, install the packages in `requirements.txt` and run the notebook.

## Code Structure and Design
- There is one main `Board` class which represents the grid.
    - The grid itself is a simple python 2D array of 1s and 0s.
    - The class has an `initialize_board` method which sets some cells to 1 as an initial game state
    - It also has the update step method which transitions current state to next state based on rules.
- In the pygame loop, we simply initialize a board, update its state and draw it. The pygame loop is very minimal and beginner friendly.
- You can play with different initialization setups by passing in different list of alive cell coordinates to the `initialize_board` method. Indexing is a bit weird and inconsistent between pygame's window coordinate system and by 2D python grid list index system. But it works.
# TIC-TAC-TOE_REACT

This project is a simple, yet classic game of Tic Tac Toe, implemented using React. The game keeps track of the current state, checks for a winner, and provides a history function to revisit previous moves.

# Learning outcome

This is not a personal project, this is for my practice while i am learning the basics of using "React.js" . This tutorial is a concept used from React-Documentation: https://react.dev/learn/tutorial-tic-tac-toe  

Take this as my progress while learning React: 

•Understood the fundamentals of React, This includes JSX, components, props, and state. Through this project, learners gain practical experience using these basic building blocks of React applications.

•Managing Component State 

•Usage of React Hooks

•Event Handling in React (props, useState etc.,.)

•Building Interactive UIs

•Understood Lifting State Up: A common pattern in React where state is lifted to the closest common ancestor of components that need it. This project provides a good example of this pattern with the state being kept in the Game component.

•Understanding Conditional Rendering (Dynamically changing components and displaying them on the localhost)

•Time Travel: The game provides a feature of going back to previous moves, which is a complex concept and will help learners understand the advanced aspects of state management.

•Building a Game Logic: Beyond just React, gain experience in building the game logic for a simple game, which includes checking for a winner.

•Working with Arrays: The project involves heavy use of JavaScript arrays, providing practice in manipulation and iteration of arrays.
this was the best practice coming from Vanilla JS. Practice of using slice() and all are different outcomes aswell 

## Components

The project is broken down into several components:

- `Square`: Represents a single square in the Tic Tac Toe board. The value prop can either be 'X', 'O', or `null`, and it includes an `onSquareClick` prop which is a callback function invoked when a square is clicked.

- `Board`: This component symbolizes the game board. It encapsulates game logic, such as determining the next player and checking for a winner, and it renders nine `Square` components. It takes `xIsNext`, `squares`, and `onPlay` as props.

- `Game`: The primary game component. It maintains the game history, an array of game states, and the current move number in its state. The `Game` component uses these to ascertain the current game state (`currentSquares`) and the player's turn (`xIsNext`). It renders the `Board` and a list of past moves that allows users to revisit previous moves.

- `calculateWinner`: A helper function that examines the current state of the game board to identify a winner by verifying all possible winning combinations (rows, columns, and diagonals).

## Features

- Two players can take turns to play the game.
- The game tracks its history, enabling players to return to any past game state.
- The winner is determined and displayed when found.

# Go Maze - Using Creational Patterns

Go Maze Game is an implementation of the maze game described in Chapter 3
("Creational Patterns") of the book "Design Patterns: Elements of Reusable
Object-Oriented Software" by Erich Gamma, Richard Helm, Ralph Johnson, and John
Vlissides. This project aims to demonstrate the application of creational
design patterns in Go.

## Introduction

The Go Maze Game is a text-based maze-solving game where the player navigates
through a maze to reach the exit. The maze is randomly generated, offering a
unique challenge with each playthrough. To solve the maze, the player can use
the arrow keys to move the character up, down, left, or right within the maze
grid. The game ends when the player successfully reaches the exit.

## Features

- **Random Maze Generation**: The game generates a random maze with walls, an
  entrance, and an exit for each new playthrough.

- **Character Movement**: Players can control the character's movement using
  the arrow keys to navigate the maze.

- **Winning Condition**: The game ends when the player reaches the exit,
  displaying a victory message.

## Installation

To run the Go Maze Game, you need to have Go installed on your machine. If you
don't have it yet, you can download and install it from the official Go
website: https://golang.org/dl/

Next, you can clone the Go Maze Game repository to your local machine using the
following command:

```bash
git clone https://github.com/writeonlycode/gomaze.git
```

## Dependencies

The Go Maze Game utilizes the `tcell` package for handling terminal input and
output. You can install it using the following `go get` command:

```bash
go get github.com/gdamore/tcell/v2
```

## Usage

To play the Go Maze game, navigate to the project's root directory and run the
following command:

```bash
go run main.go
```

Once the game starts, the maze will be displayed on the terminal, and the
player's character will be represented by the symbol "@". The player can move
the character using the arrow keys (up, down, left, right) to explore the maze
and find the exit. Upon reaching the exit, a victory message will be displayed,
and the game will end.

## Creational Design Patterns

## Creational Design Patterns

The Go Maze Game demonstrates the application of various creational design
patterns to create and manage maze-related objects. The following creational
design patterns are utilized in this project:

- **Abstract Factory Pattern**: The Abstract Factory pattern provides an
  interface for creating families of related maze objects, such as rooms,
  walls, and doors, without specifying their concrete classes. This allows the
  game to generate different types of mazes with their corresponding components
  seamlessly.

- **Builder Pattern**: The Builder pattern is used to construct the maze step
  by step, allowing different maze structures to be created based on player
  preferences. It separates the maze construction process from the rest of the
  code, providing flexibility in maze creation.

- **Factory Method Pattern**: The Factory Method pattern is employed to define
  an interface for creating maze objects but lets subclasses decide which class
  to instantiate. In the context of the game, it allows different maze types to
  be created by extending the factory method.

- **Prototype Pattern**: The Prototype pattern is possibly applied to clone
  maze-related objects for random maze generation without the need for creating
  them from scratch. It enables efficient creation of maze structures by
  copying existing objects as templates.

- **Singleton Pattern**: While not necessarily used in the maze generation
  itself, the Singleton pattern ensures that only one instance of certain
  classes, such as the maze generator or game controller, exists throughout the
  game. This can be useful for maintaining global state and resources.

These creational design patterns enhance the flexibility, reusability, and
maintainability of the Go Maze Game by encapsulating maze creation logic and
managing maze-related objects effectively. Each pattern contributes to the
overall architecture of the game and showcases the power of design patterns in
practical software development.

## Contributions

Go Maze Game is a learning project aiming to illustrate creational design
patterns in Go. While it is primarily intended for personal practice,
contributions, feedback, and bug reports are welcome.

## License

Go Maze Game is distributed under the [MIT License](LICENSE), making it
open-source and free to use.

## Acknowledgments

The creation of Go Maze Game was inspired by the "Design Patterns: Elements of
Reusable Object-Oriented Software" book, written by Erich Gamma, Richard Helm,
Ralph Johnson, and John Vlissides.


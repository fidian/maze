Maze Game (in Bash)
===================

Try to escape a maze, which is randomly generated.

![Demo](demo.gif)

The game works in Bash 3.2 and newer versions.


Installation
------------

You should download this project and install [`bpm`], then run `bpm install` to get the dependencies.


Usage
-----

There are a few options available when running `maze`.

* `--help` - Display a help message and a bit of a story behind how the player got into the maze.
* `--width=X' - Set the width of the board. Default is 20. See note about board size.
* `--height=Y` - Set the height of the board. Default is 10. See note about board size.
* `--seed=S` - Sets the random number generator's seed. Use an integer when seeding the generator.


### Board Size

The board is measured in cells, which is where the player can stand. If you imagine a sheet of graph paper, the player is always within one of the squares and the walls are drawn along the lines of the graph paper.

Multiply the width times the height to get the number of cells in the board. The time to create the maze increases with the total number of cells in the board. Below is a chart with the amount of time needed to generate mazes of different sizes on my computer.

|  Cells | Seconds |
|-------:|--------:|
|    100 |    0.09 |
|    250 |    0.25 |
|    500 |     0.7 |
|  1,000 |     1.9 |
|  1,500 |     3.7 |
|  2,000 |       6 |
|  3,000 |      12 |
|  4,000 |      21 |
|  6,000 |      44 |
|  8,000 |      82 |
| 10,000 |     120 |


License
-------

This project is placed under an [MIT License](LICENSE.md).


[`bpm`]: https://github.com/bpm-rocks/bpm

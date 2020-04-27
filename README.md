# Last Row sample data

This repository was created to share new tracking data for educational (and recreational) purposes as part of the Friends of Tracking initiative.

The data was collected mainly to make the animations posted on twitter account [@lastrowview](https://twitter.com/lastrowview), and it lacks the accuracy needed for research. Most notably, not all players are included in each play (although every player near the ball at any time is).

The main sample file is ``liverpool_2019.csv``, which contains 19 goals scored by Livepool FC in 2019.

Columns included:
* ``play``: the scoreline after the goal. The team who scored the goal is the one next to the brackets.
* ``frame``: the frame number for the current location. Data provided has 20 frames per second.
* ``player``: the id of the player. The id is consistent within a play but **not between plays**.
* ``player_num``: the player jersey number. This number is the official one, and did not change for Liverpool in 2019. You can check the corresponding names at this [wikipedia link](https://en.wikipedia.org/wiki/2019%E2%80%9320_Liverpool_F.C._season#Squad_statistics).
* ``x``, ``y``: coordinates for the player/ball. Pitch coordinates go from 0 to 100 on each axis.
* ``dx``, ``dx``: change in (x,y) coordinates from last frame to current frame
* ``z``: height, from 0 to 1.5 (only filled for the ball)
* ``bgcolor``: the main color for the team (used as background color)
* ``edgecolor`` the secondary color (used as edge color)

## Getting started

You can get a feel for the dataset by checking the Jupyter Notebook included in this repository. Basic ploting is built on top of ``matplotlib``, and animations are built with ``moviepy``.

Feel free to use the dataset for whatever purpose, but please credit the source and let us know about it!

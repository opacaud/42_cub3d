# 42_cub3d

## Project 08: Creating a Wolfenstein 3D environment from a file containing a map of zeroes and ones.

Keep in mind that this program was designed on **Ubuntu 20.04**. It was brought to my attention that it did not compiled as is on some other OS.
</br>

Run ```make``` and then ```./cubd3d maps/test.cub```
</br>

If everything goes as it does on 42 computers, a window should open, representing the character's view.
You can move using **the arrows and the letters WASD on American qwerty keyboards**.
</br>

If you open the file containing the map, you will see :

* C for **ceiling** followed by the color in RGB values separated with commas.
* F for **floor** followed by the color in RGB values separated with commas.

* NO for **North** followed by the path to the xpm file representing the texture you want to appear on the northern walls.
* SO for **South** followed by the path to the xpm file representing the texture you want to appear on the southern walls.
* EA for **East** followed by the path to the xpm file representing the texture you want to appear on the eastern walls.
* WE for **West** followed by the path to the xpm file representing the texture you want to appear on the western walls.

Note that all these six lines can be written in this order of your choosing.
</br>

Finally, you will see a series of characters representing the environment you want to evolve in. (It has to be the last information available in this file.)
* **0 are for empty space.**
* **1 are for walls.**
* **N, S, E, W is for your initial position and your orientation: facing North, South, East or West.**

Of course, the map should be surrounded by ones. Anyway, an error should appear if you do not abide by some basic rules.
Example: you can only have one character position (so only one N, S, E or W), you cannot have any other characters than spaces, 0, 1, N, S, E, W and 2 for the bonus part. Yes, there is a bonus part!
</br>
</br>

### ------------------------------BONUS------------------------------

Run ```make bonus``` and then ```./cubd3d maps/map_bonus.cub```
</br>

For this projet, we decided to implement several bonus features:
* a **minimap** indicating where you are and what your orientation is
* a detection of the **mouse** to move your orientation
* **sprites** that are, as you may have seen, represented by the new character 2 in the map file
</br>

This project was a lot of work. Not so much for the parcing part but for the projection part, using **ray casting**.
</br>

Bottom line, if you want to make video games, do not listen the bitter grown-ups saying: "You'll never use pythagorean theorem anyway..."

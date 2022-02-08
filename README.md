# 42_cub3d

## Project 08: Creating a Wolfenstein 3D environment from a file containing a map of zeroes and ones.

Please keep in mind that this project was developed on an **Ubuntu 20.04** environment.
It has been brought to my attention that compilation can be problematic on other OS.
</br>

Run ```make``` and then ```./cub3D maps/test.cub```
</br>

The files in the **maps** folder should always end with a .cub extension and are always filled with the same instructions:
* C for **ceiling** is followed by three comma-separated RGB values.
* F for **floor** is followed by three comma-separated RGB values.
* NO for **North** is followd by the path leading to the texture that will be printed on northern walls.
* SO for **South** is followd by the path leading to the texture that will be printed on southern walls.
* EA for **East** is followd by the path leading to the texture that will be printed on eastern walls.
* WE for **West** is followd by the path leading to the texture that will be printed on western walls.

Note that parcing has been done such a way that all these six elements can be given in any order.
But the last element of the file must always be the map.
</br>

The map is made of:
* **0** for empty ground
* **1** for walls
* **N, S, E or W** for the character and his or her orientation at the beginning

If the map is not valid, an error should tell you so. Examples:
* The map should have a .cub extension.
* The map should be surrounded by 1.
* There must be one and only one player.
* The map can only be made of 0, 1 and one N, S, E or W.

If everything worked out fine, a window should open, representing the character's point of view.

You can slide from side to side with the **A and D keys on an American qwerty keyboard**.
You can move front and back with the **W and S keys**, as well as **up and down arrows**.
You can pivot your point of view with the **left and right arrows**.

### Bonus

Run ```make bonus``` and then ```./cub3D_bonus maps/map_bonus.cub```

Just like before a window open. this time, you mat have noticed that a new character appeared in the map:
* **2** for animated sprites

The bonus part contain several new features:
* animated **sprites**
* motion from the **mouse**
* a **minimap**

This project was actually really fun. Seeing math coming to life was really rewarding. **Ray casting** was an interesting feature to learn.
</br>

Bottom line, if you want to make video games, **do not listen to grown-ups saying: "You will never use the pythagorean theorem anyway."**
</br>

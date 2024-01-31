# so_long (125/100)

**so_long** is a project at 42 School that involves creating a simple 2D game using the MiniLibX graphics library. The base goal is to build a game where a player navigates through a map, collects items, and reaches the exit. Having done bonuses, you have to do so while also avoiding enemies that move randomly.
## Features
- Custom implementation of a 2D game engine.
- Supports player movement with arrow keys, item collection, and map rendering.
- Integration with the MiniLibX graphics library for real-time rendering.
- Animated sprites for the character and enemies. (bonus)
- Live move counter. (bonus)

## Usage
1. Clone the repository:
   <pre>
   git clone https://github.com/Thawnder/so_long.git
   </pre>
2. Compile the so_long program:
   <pre>
   make
   </pre>
3. Run the so_long program with a map file as an argument:
   <pre>
   ./so_long map.ber
   </pre>
   Replace `map.ber` with the path to the map file you want to use. <br>
   Only small.ber and medium.ber are available in my repo right now, but you can create your own map, it is quite easy !

## Creating a map

Here are the characters needed and their interpretation: <br>
1 : Wall <br>
0 : Floor <br>
C : Collectible <br>
Z : Enemy <br>
P : Player (starting point)
E : Exit <br>
<br>
The rules are simple. The map has to be closed (have walls all around it), have at least one player, but also one collectible and one exit, which both have to be accessible to the player. <br>
If your map doesn't follow one of those rules, my program will deem it invalid. Have fun !

## Preview
<pre>
$ ./so_long maps/small.ber
</pre>

<p align="center"> <img src="So_long.gif" alt="animated" /> </p>

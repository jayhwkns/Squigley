# Squigley
Squigley is a 2D platformer that I developed during my freshman year of
college. Though far from a perfect game, it was a project I was determined
to see through to the end.

The game was developed using **Unity 2D** and **C#**, which helped reinforce
the object-oriented programming paradigm that I was learning in my classes.
I went into college hoping computer science would teach me everything I
needed to build projects like video games as a hobby. Working on *Squigley*
during my first year really got me excited to learn more and improve my skills.

Being a solo developer, I also did most of the art and music, though I also
collaborated with some friends back home I was in a band with for the song that
plays during the end-credits. This was the biggest music recording and
composition project I've done to date.

Listen to the soundtrack [here](https://www.youtube.com/watch?v=9F_9Kx1DbPY&t=1206s).

# [Free on Steam](https://store.steampowered.com/app/2822670/Squigley/)

# Commands

Type `>` to open a "Debug Terminal". Think of it as commands in Minecraft or the
command line in Valve/Quake games. Handled in `Assets/Scripts/Logic/DebugTerminal.cs`

For all commands that use coordinates, you can prefix numbers with `~` to make the
coordinates relative to your position instead of absolute.

### Debug

`>debug` displays whether `debug` (cheats) is enabled or not.

`>debug true` Enables cheats. Once enabled, they are locked on until save data is reset,
meaning you can't earn achievements. You can do `>debug false`, but uhh it never really
does anything because of this property. I didn't really think this one through.

### Pos

`>pos` displays the x and y position.

`>pos x y` Teleports the player.

### Smoothcam

`>smoothcam <true/false>` turns smoothcam on and off.

### Coin / Lives

`>coin` and `>lives` set the number of coins and lives respectively.

### Noclip

Toggles noclip. Noclip has a couple different modes. Hold shift to move at a flat speed
instead of accelerating. Hold control to lock your position to 1 unit integers.

### Time

`>time 1` Sets the timescale. Higher is faster.

### Invis

`>invis <true/false>` to explicitly make yourself invisible.

`>invis` to toggle invisibility.

This was helpful when I was recording footage for trailers.

### Obj

Place game objects.

`>obj <object id> <x> <y> {<sizeX sizeY> {<rotation>}}`

The object ID can be an integer or a string value in objNames.
`string[] objNames = {"whiteplat", "greyplat", "recthaz", "spike", "rotabox", "latchbox", "slugfield", "spdfield", "rubble", "ice","goopblock","coin", "jumpcoin", "checkpoint", "finish"};`

### Des

`>des x y` Destroys a game object at x and y coordinates.

### Bind

Rebind inputs

### Undo/Redo

`>undo` and `>redo` undoes 1 past action. You can also specify a number of actions to undo
or redo.

These are a little buggy though, so be careful.

### Void, Overworld

`>void` and `>overworld` takes you to an empty world for map building or to the main
world to actually play the game normally.

### Save / Load

`>save` when in the overworld saves the game normally. Auto-save happens on exit, so this
only does something significant when the game crashes.

`>save <mapname>` saves the objects you placed if you are in the void. 


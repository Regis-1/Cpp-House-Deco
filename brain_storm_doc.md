# Design / organisational document
For writting down ideas, features, documentation etc.

## Game design
### Theme
- House decorating game
- setting: not so modern; maybe more cottagecore side
- cosy game vibes; relaxing

### Art style / graphics
- pixel art
- 2D graphics - top down view (like _Stardew Valley_, or _To the moon_)
- tilemap
- lively, happy colors

### Mechanics / game loop
- Version 1.0:
  - changing the interior of the given house via "editor mode"
  - selecting/changing the size of the interior itself
  - selecting necessary objects from "inventory" and placing them
  - removing the objects (completely, without going back to inventory or something)
  - handling of objects with different sizes, e.g., 1-tile chair as well as 4-tiles big bed
- Version X.X:
  - all of the above
  - ...

### Deadlines
- 19.03.2023:
  - working window with input handling
  - ImGui implemented
  - basic modules with classes created

## File structure
As for the file structure, for now let's go with each class separation and eventually (and optionally) module separation. Little presentation below:

```
main directory
|-- extlibs
|   |-- SDL2
|   |-- ...
|
|-- src
|   |-- main.cpp
|   |
|   |-- Game
|   |   |-- CMakeLists.txt
|   |   |-- Game.cpp
|   |   |-- Game.hpp
|   |
|   |-- Scene
|   |   |-- CMakeLists.txt
|   |   |-- Scene.cpp
|   |   |-- Scene.hpp
|   |
|   |-- GameObject
|   |   |-- ...
|   |
|   |-- ...
|
|-- CmakeLists.txt
|-- .gitignore
```
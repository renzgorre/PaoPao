# PaoPao

A top-down pixel-art exploration game built with [HaxeFlixel](https://haxeflixel.com/). Wander through an apartment building, ride the elevator down to the street, and hang out with Chochi the dog.

This is a pre-alpha prototype.

## Features

- Explorable apartment: bedroom, bathroom, living room, hallway, elevator and ground floor, plus an outdoor area
- Chochi, an NPC dog you can talk to
- A dialogue system that reads conversations from text files
- Background music for the menu, apartment and elevator
- Main menu and an in-game options menu

## Controls

| Key | Action |
| --- | --- |
| W A S D or arrow keys | Move |
| E | Talk to Chochi |
| Enter | Advance dialogue |
| Esc | Open the options menu |

## Building

Requirements: [Haxe 4](https://haxe.org/download/) and the HaxeFlixel libraries.

```bash
haxelib install lime
haxelib install openfl
haxelib install flixel
haxelib install flixel-addons
haxelib run lime setup
```

Then build and run from the project folder:

```bash
lime test html5     # in the browser
lime test windows   # or mac / linux
```

Builds are written to `export/`.

## Project structure

| Path | Contents |
| --- | --- |
| `source/character/` | Player and NPCs (Chochi, cars) |
| `source/level/` | Level loading and each room of the apartment and outside |
| `source/dialogue/` | Dialogue box and text playback |
| `source/menu/` | Main and options menus |
| `assets/data/Maps/` | Room layouts made in [Ogmo Editor 3](https://ogmo-editor-3.github.io/) |
| `assets/data/Dialogue/` | Dialogue scripts |
| `aesprite/` | Source sprite files for [Aseprite](https://www.aseprite.org/) |
| `Project.xml` | Lime/OpenFL project configuration |

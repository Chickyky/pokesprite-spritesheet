[![MIT license](https://img.shields.io/badge/license-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT) [![npm version](https://badge.fury.io/js/pokesprite-spritesheet.svg)](https://badge.fury.io/js/pokesprite-spritesheet) ![Updated for](https://img.shields.io/badge/Updated%20for-Pok%C3%A9mon%20Sword%2FShield%20(Isle%20of%20Armor%20DLC)-blue)

# PokéSprite - generated spritesheet

This repo contains a spritesheet build automatically from the [PokéSprite project](https://github.com/msikma/pokesprite). It's designed to make it easy to add Pokémon sprites to a website.

<p align="center"><img align="center" src="docs/banner_gen8_2x.png" alt="Pokésprite Gen 8 examples banner" width="726"></p>

See [the overview page](#) for a list of all supported sprites.

## Including the library in a page

To get started, add any of these CSS files to the `<head>` of your page:

```html
<link rel="stylesheet" href="pokesprite-pokemon-gen8.css" />
<link rel="stylesheet" href="pokesprite-inventory.css" />
<link rel="stylesheet" href="pokesprite-misc.css" />
```

In most cases, you'd only want the first—this one contains **Pokémon sprites**. The second contains **inventory items**, and the third **miscellaneous sprites** of various types. How you point to the CSS files depends on how you're using this library. (TODO: add examples.)

Each CSS file has an image file of the same name that it expects to be present in the same directory.

### Displaying sprites

Sprites are accessible by adding a `<span>` with the right class name:

| HTML | Result |
|:-----|:------:|
| `<span class="pokesprite pokemon bulbasaur">` | ![Bulbasaur](https://raw.githubusercontent.com/msikma/pokesprite/master/pokemon-gen8/regular/bulbasaur.png) |
| `<span class="pokesprite pokemon bulbasaur shiny">` | ![Bulbasaur (shiny)](https://raw.githubusercontent.com/msikma/pokesprite/master/pokemon-gen8/shiny/bulbasaur.png) |
| `<span class="pokesprite ball dusk">` | ![Dusk ball](https://raw.githubusercontent.com/msikma/pokesprite/master/items/ball/dusk.png) |

## Limitations

Currently, only sprites that are meant to be displayed as *pixel art* are included in the spritesheet. There are many miscellaneous sprites that are meant to be displayed at higher resolutions, such as the Sword/Shield images for the ribbons. Putting large images in a spritesheet is generally not desirable due to the large size of the composite image. It's also less convenient for setting a custom display size, which is possible for some of these larger sprites as not all of them have a specific target size.

As a result these larger sprites are currently not part of the generated spritesheet, although more sprites will be included in a future update.

## Related projects

* [PokéSprite](https://github.com/msikma/pokesprite) – main project and image database
* [pokesprite-gen](https://github.com/msikma/pokesprite-gen) – tool that generates the content of this repo

## License

The sprite images are © Nintendo/Creatures Inc./GAME FREAK Inc.

Everything else, and the programming code, is governed by the [MIT license](http://opensource.org/licenses/MIT).

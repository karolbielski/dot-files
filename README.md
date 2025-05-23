# My Dot Files

- [AeroSpace](https://github.com/nikitabobko/AeroSpace) as tile manager
- [JankyBorders](https://github.com/FelixKratz/JankyBorders) to style frames
- [SketchyBar](https://github.com/FelixKratz/SketchyBar) to style status bar
- [Karabiner](https://karabiner-elements.pqrs.org) to map keyboard keys

## Installation

### AeroSpace

Install

```shell
brew install --cask nikitabobko/tap/aerospace
```

Copy configuration

```shell
cp aerospace/.aerospace.toml ~/.aerospace.toml
```

### JankyBorders

Install

```shell
brew tap FelixKratz/formulae
brew install borders
```

Copy configuration

```shell
cp jankyborders/bordersrc ~/.config/borders/bordersrc
```

### SketchyBar

Install

```shell
brew tap FelixKratz/formulae
brew install sketchybar
mkdir -p ~/.config/sketchybar/plugins
cp $(brew --prefix)/share/sketchybar/examples/sketchybarrc ~/.config/sketchybar/sketchybarrc
cp -r $(brew --prefix)/share/sketchybar/examples/plugins/ ~/.config/sketchybar/plugins/
curl -L https://github.com/kvndrsslr/sketchybar-app-font/releases/download/v1.0.16/sketchybar-app-font.ttf -o $HOME/Library/Fonts/sketchybar-app-font.ttf
curl -L https://github.com/kvndrsslr/sketchybar-app-font/releases/download/v1.0.20/icon_map_fn.sh -o ~/.config/sketchybar/plugins/icon_map_fn.sh
chmod +x ~/.config/sketchybar/plugins/icon_map_fn.sh
chmod +x ~/.config/sketchybar/items/front_app.sh
```

Copy configuration

```shell
cp -a sketchybar ~/.config
```

### Karabiner-Elements

Install

```shell
brew install --cask karabiner-elements
```

Copy configuration

```shell
cp -a karabiner ~/.config
```

# color-converter

This command line utility simply converts colors from hexadecimal colors to RGB
and vice versa. It aims for simplicity, portability and uses ``bc``, ``cut``
and other commands as little as possible.

Feel free to contribute to the project in any way or create an issue if you
happen to find a bug.

## Installation
```bash
$ git clone https://github.com/majjoha/color-converter.git
```

```bash
$ cd color-converter && sudo cp color-converter /usr/local/bin/color-converter
```

## Usage
### Convert a hexadecimal color to RGB
```bash
$ color-converter ff0000
#ff0000 -> rgb(255, 255, 0)
```

```bash
$ color-converter "#c71585"
#c71585 -> rgb(199, 21, 133)
```

### Convert a color in RGB to a hexadecimal value
```bash
$ color-converter 255 255 0
rgb(255, 255, 0) -> #ffff00
```

### Change luminosity of a RGB value
```bash
$ color-converter 255 255 255 -25
rgb(255, 255, 255) -> rgb(230, 230, 230)
```

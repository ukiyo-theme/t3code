# karazuri for T3 Code

The karazuri color theme for [T3 Code](https://github.com/pingdotgg/t3code).

[View the palette](https://karazuri.github.io/palette/)

## Variants

Each T3 Code theme pairs a dark variant with a light variant.

| Theme | Theme file | Dark variant | Light variant |
|---|---|---|---|
| karazuri | [karazuri.json](themes/karazuri.json) | Umi | Kami |
| karazuri Yoru | [karazuri-yoru.json](themes/karazuri-yoru.json) | Yoru | Kami |

| Variant | Background | Description |
|---|---|---|
| Umi (sea) | `#1A1A22` | Dark, with cool tones. |
| Yoru (night) | `#161514` | Darker and warmer than Umi. |
| Kami (paper) | `#D2CCBC` | Light, with a paper-colored background at about 60% brightness. |

### Umi

![Umi palette preview](https://raw.githubusercontent.com/karazuri/palette/main/assets/umi.svg)

### Yoru

![Yoru palette preview](https://raw.githubusercontent.com/karazuri/palette/main/assets/yoru.svg)

### Kami

![Kami palette preview](https://raw.githubusercontent.com/karazuri/palette/main/assets/kami.svg)

## How to use

1. From this repository, copy the theme file you want to `~/.t3/userdata/themes/`. For karazuri, run the following commands. For karazuri Yoru, use `karazuri-yoru.json` in both paths.

   ```sh
   mkdir -p ~/.t3/userdata/themes
   cp themes/karazuri.json ~/.t3/userdata/themes/karazuri.json
   ```

2. Open T3 Code settings and select **karazuri** or **karazuri Yoru**.
3. The selected theme follows the app's appearance. Dark mode uses Umi or Yoru, depending on the theme. Light mode uses Kami in both themes.

You can also ask the T3 Code agent to install `themes/karazuri.json` as the `karazuri` theme.

## Regenerating the themes

The files in `themes/` are generated from `palette.json` in [karazuri/palette](https://github.com/karazuri/palette). Make color changes in the palette repository and regenerate the theme files with the following command.

```sh
python3 ../palette/scripts/build.py t3code --out .
```

Run the command from this repository with the palette repository cloned next to it.

## License

MIT

# Ukiyo for T3 Code

The [Ukiyo](https://github.com/ukiyo-theme/palette) color theme for [T3 Code](https://github.com/pingdotgg/t3code).

T3 Code themes have one dark and one light appearance, so there are two themes:

| Theme file | Dark | Light |
|---|---|---|
| `themes/ukiyo.json` | Umi (`#1A1A22`) | Kami (`#D2CCBC`) |
| `themes/ukiyo-yoru.json` | Yoru (`#161514`) | Kami (`#D2CCBC`) |

## Install

T3 Code keeps published themes in `~/.t3/userdata/themes/`, one JSON file per theme named after its id. Copy a theme there:

```sh
mkdir -p ~/.t3/userdata/themes
cp themes/ukiyo.json ~/.t3/userdata/themes/ukiyo.json
```

You can also ask the T3 Code agent to install `themes/ukiyo.json` as the `ukiyo` theme.

## Changing the colors

Don't edit `themes/*.json` by hand. They are generated from `palette.json` in [ukiyo-theme/palette](https://github.com/ukiyo-theme/palette):

```sh
python3 ../palette/scripts/build.py t3code --out .
```

The path assumes both repos are cloned side by side.

## License

MIT

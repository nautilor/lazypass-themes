# lazypass-themes

Color themes for [lazypass](https://github.com/nautilor/lazypass). Each file in `themes/` is a drop-in `gui.theme` config using lazygit-style keys.

## Usage

Copy a theme over your lazypass config:

```sh
mkdir -p ~/.config/lazypass
cp themes/catppuccin-mocha.yml ~/.config/lazypass/config.yml
```

Or point lazypass at a theme directly:

```sh
lazypass -config ~/path/to/lazypass-themes/themes/nord.yml
```

Symlink if you want updates via `git pull`:

```sh
ln -sf "$PWD/themes/tokyonight.yml" ~/.config/lazypass/config.yml
```

## Theme format

```yaml
gui:
  theme:
    activeBorderColor:            # focused panel border (accent)
      - "#61AFEF"
      - bold
    inactiveBorderColor:          # unfocused panel border
    optionsTextColor:             # bottom keybinding hints
    selectedLineBgColor:          # highlighted row background
    selectedRangeBgColor:         # multi-select range background
    cherryPickedCommitFgColor:
    cherryPickedCommitBgColor:
    unstagedChangesColor:
    defaultFgColor:               # default text
    searchingActiveBorderColor:   # border while searching
  nerdFontsVersion: "3"
```

## Themes

| Theme | Accent |
|---|---|
| `alucard` | `#644AC9
#CFCFDE` |
| `ayu-dark` | `#59C2FF
#2D3640` |
| `ayu-light` | `#399EE6
#D5D7D9` |
| `ayu-mirage` | `#73D0FF
#3E4B59` |
| `base16-default-dark` | `#7CAFC2
#383838` |
| `base16-eighties` | `#6699CC
#515151` |
| `carbonfox` | `#78A9FF
#484848` |
| `catppuccin-frappe` | `#8CAAEE
#51576D` |
| `catppuccin-latte` | `#1E66F5
#BCC0CC` |
| `catppuccin-macchiato` | `#8AADF4
#494D64` |
| `catppuccin-mocha` | `#89B4FA
#45475A` |
| `challenger-deep` | `#91DDFF
#565575` |
| `city-lights` | `#539AFC
#333F4A` |
| `cyberpunk` | `#00FFFF
#3A3A5C` |
| `dawnfox` | `#286983
#BDBFC9` |
| `dracula` | `#BD93F9
#6272A4` |
| `edge-dark` | `#6CB6EB
#414550` |
| `everforest-dark` | `#7FBBB3
#475258` |
| `everforest-light` | `#3A94C5
#BDC3AF` |
| `github-dark` | `#58A6FF
#30363D` |
| `github-dimmed` | `#539BF5
#373E47` |
| `github-light` | `#0969DA
#D0D7DE` |
| `gruvbox-dark` | `#83A598
#504945` |
| `gruvbox-light` | `#076678
#D5C4A1` |
| `gruvbox-material` | `#7DAEA3
#45403D` |
| `hackerman` | `#00FF41
#0A4A1A` |
| `high-contrast` | `#00FFFF
#808080` |
| `horizon` | `#26BBD9
#2E303E` |
| `iceberg` | `#84A0C6
#3E445E` |
| `kanagawa-dragon` | `#8BA4B0
#625E5A` |
| `kanagawa-lotus` | `#4D699B
#C7C7D4` |
| `kanagawa` | `#7E9CD8
#54546D` |
| `light-owl` | `#4876D6
#D9D9D9` |
| `material-darker` | `#82AAFF
#424242` |
| `material-ocean` | `#82AAFF
#1F2233` |
| `material-palenight` | `#82AAFF
#3A3F58` |
| `mono-dark` | `#FFFFFF
#444444` |
| `monokai-pro` | `#78DCE8
#727072` |
| `monokai` | `#66D9EF
#75715E` |
| `mono-light` | `#000000
#BBBBBB` |
| `moonlight` | `#82AAFF
#444A73` |
| `nightfox` | `#719CD6
#39506D` |
| `night-owl` | `#82AAFF
#5F7E97` |
| `nord-light` | `#5E81AC
#D8DEE9` |
| `nord` | `#88C0D0
#4C566A` |
| `oceanic-next` | `#6699CC
#4F5B66` |
| `onedark-vivid` | `#61AFEF
#3E4452` |
| `onedark` | `#61AFEF
#3E4452` |
| `onelight` | `#4078F2
#CACAD0` |
| `oxocarbon` | `#78A9FF
#393939` |
| `palenight` | `#82AAFF
#4E5579` |
| `papercolor-dark` | `#5FAFD7
#585858` |
| `papercolor-light` | `#005F87
#BCBCBC` |
| `retro-amber` | `#FFB000
#664400` |
| `rose-pine-dawn` | `#56949F
#CECACD` |
| `rose-pine-moon` | `#9CCFD8
#44415A` |
| `rose-pine` | `#9CCFD8
#403D52` |
| `solarized-dark` | `#268BD2
#586E75` |
| `solarized-light` | `#268BD2
#93A1A1` |
| `sonokai` | `#76CCE0
#414550` |
| `spaceduck` | `#7A5CCC
#30365F` |
| `synthwave84` | `#36F9F6
#495495` |
| `tokyonight-day` | `#2E7DE9
#A8AECB` |
| `tokyonight-storm` | `#7AA2F7
#3B4261` |
| `tokyonight` | `#7AA2F7
#3B4261` |
| `tomorrow-night` | `#81A2BE
#373B41` |
| `tomorrow` | `#4271AE
#D6D6D6` |
| `ubuntu` | `#E95420
#5E2750` |
| `vscode-dark` | `#569CD6
#3C3C3C` |
| `vscode-light` | `#0000FF
#C8C8C8` |
| `zenburn` | `#8CD0D3
#5F5F5F` |

## Adding a theme

1. Copy `themes/onedark.yml` to `themes/<name>.yml`.
2. Swap the hex values.
3. Add it to the table above.

Note: palette values are approximations of each upstream scheme mapped onto lazypass's ten color slots. Tweak to taste.

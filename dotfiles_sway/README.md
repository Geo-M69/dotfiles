# dotfiles_sway

Minimal Sway setup translated from Hyprland, with Waybar and Wofi.

## Layout

- `sway/config`
- `waybar/config.jsonc`
- `waybar/style.css`
- `wofi/config`
- `wofi/style.css`
- app configs: `ghostty/`, `helix/`, `mpv/`

## Packages

Core packages are listed in `dependencies_core.txt`.
Optional packages are listed in `dependencies_extra.txt`.

Install example (Artix/Arch):

```bash
sed '/^\s*#/d;/^\s*$/d' dependencies_core.txt | xargs sudo pacman -S --needed
sed '/^\s*#/d;/^\s*$/d' dependencies_extra.txt | xargs sudo pacman -S --needed
```

## OpenRC Audio Note

Current `sway/config` starts audio with:

- `pipewire`
- `wireplumber`
- `pipewire-pulse`

If you prefer OpenRC services instead, disable those three `exec` lines in `sway/config` to avoid duplicate starts.

## Wallpaper Note

Wallpaper is loaded from:

- `$HOME/Pictures/Wallpapers/wallhaven-rqqy5m_1280x800_1.png`

If the file does not exist, the config falls back to a solid color background.

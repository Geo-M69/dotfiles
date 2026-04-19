# dotfiles_sway

Minimal Sway setup with Waybar and Wofi.

## Layout

- `sway/config`
- `waybar/config.jsonc`
- `waybar/style.css`
- `wofi/config`
- `wofi/style.css`
- app configs: `ghostty/`, `helix/`, `mpv/`

## Packages

Core packages in `dependencies_core.txt` are required for the current default config to run as written (including Waybar audio + icon font support).
Optional packages in `dependencies_extra.txt` are quality-of-life additions and integrations.

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

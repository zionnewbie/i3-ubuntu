# i3 Ubuntu Configuration

This repository provides a ready-to-use set of configuration files and setup instructions for running the i3 window manager on Ubuntu. It includes custom themes, fonts, Polybar, Rofi, and various scripts to enhance your workflow.

> **Note:**  
> This setup is a personal project and may not be fully polished. Some configurations and scripts are adapted from community sources.  
> **Use at your own risk!** If you encounter issues, GOOD LUCK Troubleshooting! o.o sorry mate ! i myself have no clue what the issue maybe!.

---

## Required Packages

Install these packages with `sudo apt install`:

- `i3` – Tiling window manager
- `rofi` – Application launcher and window switcher
- `compton` – Compositor for transparency and effects
- `nitrogen` – Wallpaper manager
- `polybar` – Customizable status bar
- `arandr` – Display configuration tool (for generating `xrandr` scripts)
- `playerctl` – Media player controller (Polybar integration)
- `dunst` – Notification daemon
- `fonts-noto` – Noto Sans font
- `pulseaudio-utils` – Audio control utilities
- `network-manager` & `network-manager-gnome` – Network management and tray applet
- `git` – Version control

### Additional Package Details

- **feh:** Alternative to Nitrogen for wallpapers; supports scripting.
- **lxappearance:** Easily change GTK themes and icons.
- **xclip:** Enables terminal-to-GUI clipboard operations.
- **pulseaudio-utils:** Tools like `pactl` for Polybar audio modules.
- **network-manager:** Essential for network management.
- **flameshot:** Screenshot and annotation tool.
- **unclutter:** Hides the mouse cursor after inactivity.

---

## Configuration Overview

- **i3status:** Replaced by Polybar for a more customizable status bar.
- **Nitrogen & Compton:** Autostart for wallpaper and compositing.
- **Wallpapers:** Not included; i have some in my `./wallpapers/` folder or use your own .
- **Rofi:** Themed application launcher.
- **Display Setup:** Use arandr to generate `xrandr` scripts for multi-monitor setups.
- **Fonts:** Noto Sans for a clean, readable interface.
- **Polybar:** Displays system info, audio, network, and more.
- **Dunst:** Handles notifications.
- **Flameshot:** For screenshots and annotations.
- **LXAppearance:** Change GTK themes and icons.
- **Unclutter:** Hides the mouse cursor when idle.

---

## Notes

- Some scripts and configs are adapted and customized for this setup.
- This repository is a starting point for your own i3 customization.
- Contributions and suggestions are welcome!

---

## Installation Steps

1. **Update your system:**

   ```sh
   sudo apt update && sudo apt upgrade
   ```

2. **Install all required packages:**

   ```sh
   sudo apt install i3 rofi compton nitrogen polybar arandr playerctl dunst fonts-noto feh lxappearance xclip pulseaudio-utils network-manager network-manager-gnome flameshot git unclutter
   ```

3. **Clone this repository:**

   ```sh
   git clone https://github.com/zionnewbie/i3-ubuntu.git
   ```

4. **Copy configuration files to your home directory:**

   ```sh
   cp -r i3-ubuntu/.config ~/
   ```

5. **Log out and select i3 from your login manager.**

---

## Customization Tips

- Edit `~/.config/i3/config` for keybindings and startup apps.
- Use `lxappearance` for GTK themes and icons.
- Modify Polybar in `~/.config/polybar/config`.
- Set wallpapers with Nitrogen or Feh.
- Tweak Rofi themes in `~/.config/rofi/`.

---

## Troubleshooting

- If Polybar or Compton fails, check `~/.xsession-errors`.
- For display issues, re-run `arandr` and update startup scripts.
- Missing fonts or icons? Install additional packages as needed.
- You can use this to learn or understand stuff but this project itself is not perfect.

---

Enjoy your personalized i3 Ubuntu desktop!

# Linux Dotfiles — BSPWM & Polybar

A personalized Linux desktop configuration built on Linux Mint, featuring BSPWM, Polybar, and a keyboard-driven workflow.

This project focuses on minimalism, productivity, system customization, and efficient navigation through a lightweight tiling window manager.

## Desktop Preview

![Desktop Preview](screenshot.png)

![Alternative Desktop Preview](screenshot2.png)

## Features

- Lightweight tiling window management with BSPWM.
- Customizable status bar using Polybar.
- Keyboard-driven navigation through SXHKD.
- GPU-accelerated terminal using Kitty.
- Window compositing and visual effects with Picom.
- Application launching through Rofi.
- Custom display and appearance configurations.

## Technologies & Tools

| Tool | Purpose |
|------|---------|
| Linux Mint | Operating system |
| BSPWM | Tiling window manager |
| Polybar | Desktop status bar |
| SXHKD | Keyboard shortcut manager |
| Kitty | Terminal emulator |
| Picom | Window compositor |
| Rofi | Application launcher |
| Neofetch | System information display |
| Xrandr | Display configuration |
| Shell | Scripting and automation |
| Git | Version control |

## Repository Structure

```text
.
├── bspwm/         # Window manager configuration
├── kitty/         # Terminal configuration
├── neofetch/      # System information customization
├── picom/         # Compositor configuration
├── polybar/       # Status bar configuration
├── rofi/          # Application launcher configuration
├── spicetify/     # Spotify customization
├── sxhkd/         # Keyboard shortcut configuration
├── xrandr/        # Display configuration
├── screenshot.png
├── screenshot2.png
└── README.md
```

## Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Super + Enter` | Launch terminal |
| `Super + Q` | Close window |
| `Super + Space` | Toggle floating mode |
| `Super + H/J/K/L` | Move window focus |
| `Super + Shift + H/J/K/L` | Move window |
| `Super + R` | Open application launcher |

Keyboard shortcuts can be customized through the SXHKD configuration.

## Installation

> [!WARNING]
> These dotfiles are designed for a personal Linux desktop environment. Review the configuration files and back up your existing settings before installation. Some configurations may require adjustments for your hardware or Linux distribution.

### 1. Install dependencies

On Linux Mint or other compatible Debian-based distributions:

```bash
sudo apt update
sudo apt install bspwm sxhkd polybar kitty rofi feh picom git
```

JetBrains Mono Nerd Font is recommended for the intended appearance.

### 2. Clone the repository

```bash
git clone https://github.com/adamarifdev/dotfiles-bpswm.git ~/dotfiles
```

### 3. Back up existing configurations

```bash
cp -a ~/.config ~/.config-backup-$(date +%Y%m%d-%H%M%S)
```

### 4. Install the configurations

Review the repository files before copying the required configurations into `~/.config/`.

```bash
mkdir -p ~/.config

cp -r ~/dotfiles/bspwm ~/.config/
cp -r ~/dotfiles/sxhkd ~/.config/
cp -r ~/dotfiles/polybar ~/.config/
cp -r ~/dotfiles/kitty ~/.config/
cp -r ~/dotfiles/picom ~/.config/
cp -r ~/dotfiles/rofi ~/.config/
```

### 5. Configure permissions

If present, ensure the startup scripts have executable permissions:

```bash
chmod +x ~/.config/bspwm/bspwmrc
chmod +x ~/.config/polybar/launch.sh
```

### 6. Start the desktop session

Log out of your current desktop session, select BSPWM from the login screen, and log back in.

Adjust display settings, file paths, fonts, and other preferences as needed.

## Project Objectives

This project explores several areas of Linux system customization:

- Linux desktop configuration and management.
- Shell scripting and automation.
- Keyboard-driven productivity workflows.
- Integration of independent desktop components.
- Configuration management using Git.

## Author

**Adam Arif**

Software Engineering Student  
University of Doha for Science and Technology  
Doha, Qatar

- [GitHub](https://github.com/adamarifdev)
- [LinkedIn](https://www.linkedin.com/in/adamarifdev/)

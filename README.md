# 🎙️ Alastor's "Radio Demon" Dotfiles
### *"Smile, my dear! You’re never fully dressed without a beautiful desktop!"*

This repository contains my personal **Arch Linux + Hyprland** configuration. It is themed after the Radio Demon himself, **Alastor** from *Hazbin Hotel*, featuring a "Blood & Charcoal" aesthetic, custom animations, and rounded corners.

---

## 📸 Aesthetic Profile
* **Colors:** Deep Crimson (`#AF0000`), Dark Maroon (`#4A0000`), and Onyx Black.
* **Window Borders:** 3px thick blood-red gradients at 45°.
* **Rounding:** 12px corners for a refined, modern look.
* **Effects:** Blood-red shadow glows and custom "sliding" animations.
* **Transparency:** 0.98 active opacity / 0.85 inactive opacity.

---

## 📦 Prerequisites & Dependencies

Install the following packages:

### Essential System Packages (Pacman)
```bash
sudo pacman -S git hyprland hyprpaper waybar kitty dolphin wofi qt6ct gnu-stow ttf-jetbrains-mono-nerd noto-fonts-emoji polkit-kde-agent

```

---

## 🚀 Installation Instructions

### Step 1: Clone the Repository

Clone the configuration files into a hidden directory in your home folder.

```bash
git clone [https://github.com/Nexus29/PersonalDotFiles.git](https://github.com/Nexus29/PersonalDotFiles.git) ~/.dotfiles
cd ~/.dotfiles

```

### Step 2: Prepare Your Config Directory

Hyprland looks for configs in `~/.config/hypr`. Ensure the folder exists and is empty of conflicting files.

```bash
mkdir -p ~/.config/hypr
mkdir -p ~/.config/waybar
mkdir -p ~/.config/kitty
mkdir -p ~/.config/wofi

```

### Step 3: Set the Wallpaper

Ensure your wallpaper image path in `hyprpaper.conf` matches where you saved your Alastor wallpaper. Then, launch the service:

```bash
hyprpaper &

```

---

## 📂 Repository Structure

For `stow` to work correctly, ensure your repository follows this layout:

```text
.
├── .config/
│   ├── hypr/
│   │   └── hyprland.conf
│   ├── waybar/
│   │   ├── config
│   │   └── style.css
│   └── kitty/
│       └── kitty.conf
└── README.md

```

---

## 🎹 Keybindings

The **Super** (Windows) key is the `$mainMod`.

| Keybind | Action |
| --- | --- |
| `Super + Q` | Open Terminal (Kitty) |
| `Super + C` | Kill Active Window |
| `Super + E` | Open File Manager (Dolphin) |
| `Super + R` | Open App Menu (Wofi) |
| `Super + V` | Toggle Floating Mode |
| `Super + 1-4` | Workspaces 1-4 |
| `Super + 5` | Workspace 10 (Custom Bind) |
| `Super + M` | Exit Hyprland |

---

## 🛠️ Troubleshooting

* **No Red Borders?** Ensure `hyprland.conf` has the correct `col.active_border` hex codes.
* **Icons Missing?** Install `ttf-jetbrains-mono-nerd` and restart your session.
* **Apps look white?** Run `qt6ct`, change the style to "Fusion" or "Breeze-Dark," and apply.

---

## 📻 Disclaimer

*Hazbin Hotel and Alastor are property of Vivienne "VivziePop" Medrano. This is a fan-made configuration for personal use.*

**"Stay Tuned..."**

---

### 🤝 Contribute & Upgrade

I am always looking to refine the Radio Demon experience! If you use these configurations and find a way to make the animations smoother, the CSS more gothic, or the scripts more efficient, **please help me upgrade this!** Feel free to open an **Issue** or submit a **Pull Request**. Let's make this the best Hazbin-themed desktop on Arch!

---

### 👤 Author

* **Giovanni Pio Lancellotta** - [Nexus29](https://github.com/Nexus29)
* `42 Student ID:` **glancell**
* `Personal Website:` *Coming Soon!*

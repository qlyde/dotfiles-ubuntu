# dotfiles

I installed Ubuntu 22.04 onto this partition in late September so I'm still early on in configuring my workspace but here is me documenting it along the way. I am doing this partially in case I get a new machine and want to port over my setup.

Currently I run a triple-boot X1 Carbon 7: Windows 10, Ubuntu 22.04 (old) and Ubuntu 22.04 (new).

![Desktop](Desktop.png)

## Ubuntu / GNOME

- **DE:** GNOME 42.4
  - Extensions:
    - **ArcMenu** - App Grid replacement, "start menu" app launcher, highly configurable (`Super` binded to ArcMenu, `Super+Space` binded to app search menu)
    - Blur my Shell
    - **Dash to Panel** - Moves dash to panel, highly configurable
    - Internet Radio - Listen to the radio via the panel
    - Net speed Simplified - For monitoring internet download/upload speeds
    - OpenWeather - For weather information
    - Refresh Wifi Connections - For a refresh button when searching for Wi-Fi networks
    - **Tiling Assistant** - For better/configurable snap assist and window tiling
    - **User Themes**
    - Vitals - For monitoring system vitals (load, mem, etc.)
  - **Note:** App Grid and Activities can still be used with the `Super+A` and `Super+S` keys respectively
    - Alphabetical App Grid - Sorts App Grid alphabetically (removed in GNOME 3.38)
    - Favourites in AppGrid - Keeps favourited applications in AppGrid (removed in GNOME 40)
  - **Note:** Disable Ubuntu AppIndicators and Ubuntu Dock (default System Extensions)
- **Terminal Emulator:** alacritty
  - [Theme](https://github.com/eendroroy/alacritty-theme): gruvbox_dark
- **Shell:** zsh (Oh My Zsh)
  - Theme: [powerlevel10k](https://github.com/romkatv/powerlevel10k)
  - Plugins:
    - [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)
    - [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)
- **Files:** nautilus (default)
- **Bar:** GNOME - Dash to Panel, etc.
- **Applications:** GNOME - ArcMenu
- **GTK Theme:** [Gruvbox-Dark-B](https://github.com/Fausto-Korpsvart/Gruvbox-GTK-Theme)
  - For themes to work for both GTK3 and GTK4 applications in GNOME 42, we need both `~/.themes/` and `~/.config/gtk-4.0/gtk.css`.
  - These have been checked in. By default the theme messes up Dash to Panel, so I had to modify `~/.themes/Gruvbox-Dark-B/gnome-shell/gnome-shell.css` to disable some panel styling.
- **Icons:** Yaru-dark (default)
- **Wallpaper:** [gruvbox11](https://github.com/Fausto-Korpsvart/Gruvbox-GTK-Theme/blob/master/wallpapers/gruvbox11.png)

<details>
  <summary><b>Packages:</b></summary>
  <ul>
    <li>apt (<code>apt-mark showmanual</code>)</li>
    <ul>
      <li>
        cmake pkg-config libfreetype6-dev libfontconfig1-dev libxcb-xfixes0-dev
        libxkbcommon-dev python3 <b>(alacritty dependencies)</b>
      </li>
      <li>
        build-essential git cmake cmake-data pkg-config python3-sphinx
        python3-packaging libuv1-dev libcairo2-dev libxcb1-dev libxcb-util0-dev
        libxcb-randr0-dev libxcb-composite0-dev python3-xcbgen xcb-proto
        libxcb-image0-dev libxcb-ewmh-dev libxcb-icccm4-dev
        <b>(polybar dependencies)</b>
      </li>
      <li>
        libxcb-xkb-dev libxcb-xrm-dev libxcb-cursor-dev libasound2-dev
        libpulse-dev i3-wm libjsoncpp-dev libmpdclient-dev libcurl4-openssl-dev
        libnl-genl-3-dev <b>(polybar optional dependencies)</b>
      </li>
      <li>
        gir1.2-gst-plugins-bad-1.0 gir1.2-gst-plugins-base-1.0
        gstreamer1.0-plugins-ugly gstreamer1.0-plugins-bad
        <b>(Internet Radio dependencies)</b>
      </li>
      <li>gir1.2-gtop-2.0 lm-sensors <b>(Vitals dependencies)</b></li>
      <li>build-essential</li>
      <li>code (VSCode, .deb from web)</li>
      <li>curl</li>
      <li>dconf-editor (GUI editor for dconf and gsettings)</li>
      <li>discord (Discord, .deb from web)</li>
      <li>git</li>
      <li>gnome-shell-extension-manager (for installing GNOME extensions)</li>
      <li>gnome-tweaks (for tweaking GNOME)</li>
      <li>google-chrome-stable (Google Chrome, deb from web)</li>
      <li>gparted (GNOME partition editor)</li>
      <li>grep</li>
      <li>gzip</li>
      <li>htop</li>
      <li>micro (terminal-based text editor)</li>
      <li>neofetch (for system info)</li>
      <li>python3-pip</li>
      <li>spotify-client (Spotify, from Spotify repository)</li>
      <li>stress (for imposing load on system)</li>
      <li>tmux (terminal multiplexer)</li>
      <li>tree (list directories in a tree format)</li>
      <li>tty-clock (a terminal clock)</li>
      <li>zsh</li>
    </ul>
    <li>pip (<code>pip list --user</code>)</li>
    <ul>
      <li>Pygments (for colorize omz plugin)</li>
    </ul>
    <li>source/git</li>
    <ul>
      <li>alacritty</li>
      <li>polybar</li>
      <li>powerlevel10k</li>
    </ul>
    <li>web</li>
    <ul>
      <li>rustup</li>
    </ul>
  </ul>
</details>

# dotfiles

## Ubuntu / GNOME

* **DE:** GNOME 42
  * *Extensions:*
    * **ArcMenu** - App Grid replacement, like a start menu (Super binded to ArcMenu, Super+Space binded to app search)
    * **Dash to Panel** - Moves dock to panel/status bar, highly configurable
    * Internet Radio - Listen to the radio via the status bar
    * Net speed Simplified - For monitoring internet download/upload speeds
    * OpenWeather - For weather information
    * Refresh Wifi Connections - For a refresh button when searching for Wi-Fi networks
    * **Tiling Assistant** - For better/configurable snap assist
    * Vitals - For monitoring system vitals (load, mem, etc.)
    * **Note:** App Grid and Activities can still be used with Super+A and Super+S keys
      * Alphabetical App Grid - Sorts App Grid alphabetically
      * Favourites in AppGrid - Keeps favourited applications in AppGrid (removed in GNOME 40?)
* **Terminal Emulator:** alacritty
  * *[Theme](https://github.com/eendroroy/alacritty-theme):* gruvbox_dark
* **Shell:** zsh (Oh My Zsh)
  * *Theme:* [powerlevel10k](https://github.com/romkatv/powerlevel10k)
  * *Plugins:*
    * [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)
    * [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)
* **Files:** nautilus (default)
* **Bar:** GNOME extensions - Dash to Panel, ...
* **Applications:** GNOME extensions - ArcMenu
* **GTK/Icons:** Yaru-blue-dark/Yaru-blue (default)
<details>
  <summary><b>Packages:</b></summary>
  <ul>
    <li>apt (<code>apt-mark showmanual</code>)</li>
      <ul>
        <li>cmake pkg-config libfreetype6-dev libfontconfig1-dev libxcb-xfixes0-dev libxkbcommon-dev python3 (alacritty deps)</li>
        <li>build-essential git cmake cmake-data pkg-config python3-sphinx python3-packaging libuv1-dev libcairo2-dev libxcb1-dev libxcb-util0-dev libxcb-randr0-dev libxcb-composite0-dev python3-xcbgen xcb-proto libxcb-image0-dev libxcb-ewmh-dev libxcb-icccm4-dev (polybar deps)</li>
        <li>libxcb-xkb-dev libxcb-xrm-dev libxcb-cursor-dev libasound2-dev libpulse-dev i3-wm libjsoncpp-dev libmpdclient-dev libcurl4-openssl-dev libnl-genl-3-dev (polybar optional deps)</li>
        <li>gir1.2-gst-plugins-bad-1.0 gir1.2-gst-plugins-base-1.0 gstreamer1.0-plugins-ugly gstreamer1.0-plugins-bad (Internet Radio deps)</li>
        <li>gir1.2-gtop-2.0 lm-sensors (vitals)</li>
        <li>build-essential</li>
        <li>code (VSCode, deb from web)</li>
        <li>curl</li>
        <li>dconf-editor</li>
        <li>git</li>
        <li>gnome-shell-extension-manager</li>
        <li>gnome-tweaks</li>
        <li>google-chrome-stable (deb from web)</li>
        <li>gparted</li>
        <li>grep</li>
        <li>gzip</li>
        <li>htop</li>
        <li>micro</li>
        <li>neofetch</li>
        <li>python3-pip</li>
        <li>stress</li>
        <li>tree</li>
        <li>zsh</li>
      </ul>
    <li></li>
      <ul>
        <li></li>
      </ul>
    <li>pip (<code>pip list --user</code>)</li>
      <ul>
        <li>Pygments (for colorize omz plugin)</li>
      </ul>
    <li>git</li>
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

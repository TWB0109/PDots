# coffee gruvbox i3 | dotfiles 
messy configuration files of an unemployed Linux lover

<img style="box-shadow: 0px 0px 10px #000;" src="./.assets/fakebusy.png">

# dependencies: 
* [GNU Stow](https://gnu.org/software/stow)
* [betterlockscreen](https://github.com/pavanjadhaw/betterlockscreen) for the autolock script (But you can edit the script to use your own screen locker)
* [mpd](https://github.com/MusicPlayerDaemon/MPD) & [mpc](https://github.com/MusicPlayerDaemon/mpc) for the tmux tmux-mpd script (But if you have ncmpcpp you'll obviously have them)
* [kunst](https://github.com/sdushantha/kunst) & [sxiv](https://github.com/muennich/sxiv) for Mpd cover
* [tpm](https://github.com/tmux-plugins/tpm) for tmux plugins  
* the scripts needed are in [scripts](scripts/.scripts)
* the colorscheme (located in [alacritty](alacritty/.config/alacritty/)) may be achieved with ```wal --theme <path_to_the_json_colorscheme>```

# installation:
1. Clone the repo
    ```bash
    git clone https://github.com/TWB0109/PDots.git
    ```
  
2. Install GNU Stow
  * Arch Linux and derivates
    ```bash
    pacman -S stow
    ```
    
  * Ubuntu and derivates
    ```bash
    apt-get install stow
    ```
    
3. Backup all the files that you don't want to lose (e.g your .vimrc, .xresources, .tmux.conf, .config/i3/config, .config/polybar/config, etc.)
 
4. Delete the files in your home directory that you want to stow.
 
5. Stow the repo
   ```bash
   cd PDots
   stow *
    ```

# notes:
GNU stow will symlink the files in the repo to the respective files in your system


Master-Stack Layout

https://github.com/user-attachments/assets/da80c6d1-b9a5-44c4-b738-6421365e6aa5


Scroller Layout

https://github.com/user-attachments/assets/2ff96868-b276-4fa1-b4d7-87bdc36beb3c



# feature
- dwl ipc support
- maxmize fullscreen
- swap window by direction
- swith to next not empty-workspace/workspace
- move window to next not empty-workspace/workspace
- swith focus by direction
- wheel/button + mod key bind
- hycov like overview
- numlock state pre-set in config
- portal fix for obs(use hyprland-portal)
- master layout support new_on_top
- foreign-toplevel support(dunst,waybar wlr taskbar)
- acitve on focus/urgent support
- hide empty button in waybar
- support minimize window by click waybar
- support minimize window by keyboard
- sway scratchpad support 
- window pin mode support
- text-input-v2
- window move/open animaition
- workspace switch animaition
- window close animaition
- custom mov/open/tag animaition sppeed
- fade in animation
- alt-tab switch window like gnome
- niri like scroller layout


## suggest tools
```
yay -S wofi foot xdg-desktop-portal-wlr swaybg waybar wl-clip-persist cliphist wl-clipboard wlsunset

```

# install 
# wlroots(0.17)
```
git clone -b 0.17.4 https://gitlab.freedesktop.org/wlroots/wlroots.git
cd wlroots
meson build -Dprefix=/usr
sudo ninja -C build install

git clone https://github.com/DreamMaoMao/maomaowm.git
cd maomaowm
meson build -Dprefix=/usr
sudo ninja -C build install

# set your autostart app ih this
mkdir -p ~/.config/maomao/

# some suggest config
cp autostart.sh ~/.config/maomao/
cp waybar ~/.config/maomao/ -r 
cp wofi ~/.config/maomao/ -r 
cp wallpaper ~/.config/maomao/ -r


```

# config
> [!NOTE]
> The configuration file is located in `config.h`. This file is generated every time the `meson build` command is executed. If the file already exists, it will not be regenerated. If you encounter compilation issues after updating, please try to remove this file and the `build folder`, then rerun the `meson build` command.

# thanks for some refer repo 
https://github.com/dqrk0jeste/owl - for window animation implementation code
https://github.com/djpohly/dwl - for base dwl code


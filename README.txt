# polybar-archcraft-keyboards-custom

# copy all file into respective dirs
> cp -r ./keyboards ~/.config/openbox/polybar/
> chmod +x ~/.config/openbox/polybar/keyboards/scripts/polywins.sh

> sudo cp -r ./anime /usr/share/backgrounds/
> sudo cp -r ./Backgrounds /usr/share/sddm/themes/archcraft/
> sudo cp -r ./theme.conf /usr/share/sddm/themes/archcraft/

> cp -r ./picom.conf ~/.config/
> cp -r ./config.rasi ~/.config/rofi/


# betterlockscree backgrounds
> betterlockscreen -u /usr/share/backgrounds/anime/

# Change style to "keyboards"
# Openbox Theme Sweet-Dark

# Icons
> yay -S candy-icons-git sweet-folders-icons-git

# Then go to the Settings Manager >> Appearance
# Chose Sweet-{Style}
# candy-icons are already inherited in the index.theme file of the Sweet-Folders

# In my xfce4-keyboard there where only Azerbaijany (Cyrilic)
# First check Settings Manager >> Keyboard >> Layout >> Add
# to see, if what you need is there already
# If no, to add Azerbaijany Latin one

> sudo cp -r ./evdev.xml > /usr/share/X11/xkb/rules/

# You can add other layouts to the menu, if they are defined in the /usr/share/X11/xkb/symbols/<layout> file.
# xkb_symbols should be added inside of <name></name> tag, in the <variant></variant> tag
# Example:
<variant>
  <configItem>
    <name>latin</name>
    <description>Azerbaijani</description>
  </configItem>
</variant>

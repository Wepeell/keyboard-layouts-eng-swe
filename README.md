# Keyboard layouts for Swedish (for Windows & Linux)
This layout consists of two different variants. They are primarily intended for 104-key ANSI keyboards but should work fine on 105-key ISO layouts too. 

It is based on the standard US layout but with Swedish characters added, as well as other characters that are included in the standard Swedish layout but not in the US layout. I avoided as many duplicates as possible with the exception of characters that are already duplicated in the standard Swedish layout and dead keys. 

## US-SE variant
The base and Shift layer is standard US layout. The AltGr and AltGr + Shift contains characters from the Swedish layout.

Base:  
![US-SE Base](Windows/US-SE/Previews/US-SE%20Base.png)

Base Shift:  
![US-SE Base Shift](Windows/US-SE/Previews/US-SE%20Base%20Shift.png)

AltGr:  
![US-SE AltGr](Windows/US-SE/Previews/US-SE%20AltGr.png)

AltGr Shift:  
![US-SE AltGr Shift](Windows/US-SE/Previews/US-SE%20AltGr%20Shift.png)

## SE-US variant
This variant has four of the keys around the Enter key inverted.

Base:  
![SE-US Base](Windows/SE-US/Previews/SE-US%20Base.png)

Base Shift:  
![SE-US Base Shift](Windows/SE-US/Previews/SE-US%20Base%20Shift.png)

AltGr:  
![SE-US AltGr](Windows/SE-US/Previews/SE-US%20AltGr.png)

AltGr Shift:  
![SE-US AltGr Shift](Windows/SE-US/Previews/SE-US%20AltGr%20Shift.png)

## Install
### Windows
1. Download the `Installer` folders
2. Run `setup.exe`

Alternatively, download the `.klc` source files and compile them with `Microsoft Keyboard Layout Creator`.

_Note: Only tested on Windows 10 Pro._

### Linux
1. Download the `xkb` folder
2. Place the `xkb` folder in `~/.config` as such:
   ```bash
   /home/$USER/.config/xkb/rules/evdev.xml
   /home/$USER/.config/xkb/symbols/se
   /home/$USER/.config/xkb/symbols/us
   ```
_Note: Only tested on Fedora KDE Plasma, Fedora Kinoite, Aurora and Bazzite (KDE Plasma version)._

_I could not get these overrides to work in Linux Mint. I don't know if that was an issue with Mint or the desktop environment. If you know a solution let me know._

_Otherwise, you have to install the layouts by modifying the files in `/usr/share/X11/xkb/rules` and `/usr/share/X11/xkb/symbols` by appending the contents of these layouts to the system files._

## Acknowledgments
Thanks to alexriss for this conversion script: https://github.com/alexriss/keyboard-layout-converter

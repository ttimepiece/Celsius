<div align="center">
  
  ![Celsius logo](https://github.com/ttimepiece/Celsius/blob/main/SovCastle.webp)
  
  A fast, lightweight panel that lives within your terminal.
  
  ![Python](https://img.shields.io/badge/python-%233670A0.svg?style=for-the-badge&logo=python&logoColor=ffdd54)
  ![macOS](https://img.shields.io/badge/mac%20os-%23000000.svg?style=for-the-badge&logo=macos&logoColor=F0F0F0&logoSize=auto)
  ![Linux](https://img.shields.io/badge/Linux-%23FCC624.svg?style=for-the-badge&logo=linux&logoColor=black)
  

  ##
  
  **Widgets:** `Quotes, drives, download/upload speed, wifi, local IP, battery, directory, timezone, time, calendar, sleep schedule`
  
  ##

  
</div>

![Preview](https://raw.githubusercontent.com/ttimepiece/Celsius/refs/heads/main/preview.gif)



#### Installation for mac/linux:
```
pipx install celsius                             ## Install Celsius
echo "your phrase here" >> ~/"${SHELL##*/}rc"    ## Autostart Celsius
nano $HOME/.config/celsius/celsius.conf          ## Customize widgets to your liking
```




#### Commands:
 

> Celsius is built to replace your panel with an intuitive CLI interface: `celsius`

```
celsius                 ## Spawns the panel
exit                    ## Closes the panel
celsius --dash          ## Displays a static dashboard
```
**Other arguments:** `--speed [int] --loop --theme [name] --help`

##

#### Themes and configuration:
```
## Config file can be edited with:
nano $HOME/.config/celsius/celsius.conf
```

<details>
<summary>Custom themes</summary>

> *New colors can be added by modifying* *celsius.conf*

```
THEMES = {"claw": _theme((222, 115, 86), "mauve_twilight": _theme((...
```
*To create custom themes, add a new entry while respecting the format.*
* The colors taken will follow this order: `Accent text, box borders, muted text, panel color`
</details>
<details>
<summary>Configuration options</summary>


> *The .config gives users full control over celsius*

* Custom messages can be displayed on the panel by editing: `QUOTES = {"Celsius panel", "..."}`
* The divider that separates widgets can be modified: `DIVIDER = "|"`
* The speed at which the widgets scroll can also be modified: `SPEED = "4.5"`

**Widgets can be toggled with:**
```
WIDGETS: {
battery       : false,
local_ip      : false,
date          : false,
timezone      : false,
network_speed : false,
time          : false}
```
</details>

---
<details>
<summary>Q&A</summary>
  
  > Commonly asked questions:
  
  &nbsp;&nbsp;&nbsp;Q. **What does Celsius do?** *Celsius is a CLI panel that offers easy access to information for minimalist and bare-bones Linux systems.*

  &nbsp;&nbsp;&nbsp;Q. **Can it replace my wm's boring panel?** *It's built as a drop-in replacement for most panels. However it lacks an app menu, check out **rofi***

  &nbsp;&nbsp;&nbsp;Q. **How customizable is it?** *Most aspects of the bar can be tweaked in .conf, additionally it supports extensions and addons*
   
---
</details>

<details>
<summary>Widgets</summary>
  
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;✒︎` Widgets are all organized in .../celsius/providers/`

  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;i.  Any .py file added in that directory will run if it's listen in the .config 'WIDGETS' list
  
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ii. For custom widgets and extensions use `clock.py` as a guideline.

</details>

Licensed under MIT. Please check 'LICENSE' for more information.


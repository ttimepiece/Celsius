<div align="center">
  
  ![Celsius logo](https://github.com/ttimepiece/Celsius/blob/main/SovCastle.webp)
  
  A fast, lightweight panel that lives within your terminal.
  
  ![Python](https://img.shields.io/badge/python-%233670A0.svg?style=for-the-badge&logo=python&logoColor=ffdd54)
  ![Linux](https://img.shields.io/badge/Linux-%23FCC624.svg?style=for-the-badge&logo=linux&logoColor=black)


  ##
  
  **Widgets:** `Quotes, download/upload speed, wifi, local IP, battery, directory, timezone, time, calendar, sleep schedule`
  
  ##

  
</div>





**Installation:**

Linux/mac devices:

`
pipx install celsius
`

![Screenshot 1](https://github.com/ttimepiece/Celsius/blob/main/screenshot1.webp)

## Usage:
> Celsius is built to replace your panel with an intuitive CLI interface: `celsius --bar`

```
celsius --bar    ## Spawns the panel
exit             ## Closes the panel

celsius          ## Displays a static dashboard
celsius --loop   ## Displays a dashboard that updates in real time
```
Other arguments: `--speed [int] --theme [name] --help`

![Screenshot 2](https://github.com/ttimepiece/Celsius/blob/main/screenshot%204.webp)


## Themes and configuration:
The theme can be changed by modifying DEFAULT_THEME at: `$HOME/.config/celsius.conf`


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


> *The .config gives users full control over celsius --bar*

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
  Celsius displays essential information for minimalist Linux distros, it can show:

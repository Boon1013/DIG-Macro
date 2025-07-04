# DIG Macro
<p align="center">
  <img width="80%" src="https://raw.githubusercontent.com/Boon1013/DIG-Macro/refs/heads/storage/showcase.gif" alt="Showcase video"> <br />
  <b>Auto minigame macro for <a href="https://www.roblox.com/games/126244816328678/DIG" target="_blank">DIG</a>.</b>
</p>

> [!NOTE]
> Do not expect this macro to succeed every time it attempts to dig.

> [!WARNING]
> **This macro will missclick and could end your streak!** It may also fail frequently in rare/specific situations.

## Requirements
 * [Python](https://www.python.org/) **[Recommended version: 3.13]**
 * [wmctrl](https://github.com/saravanabalagi/wmctrl) **[Only for Linux users]**
    - On Debian/Ubuntu: `sudo apt-get install wmctrl`
    - On Fedora: `sudo dnf install wmctrl`

## Installation
1.  **Clone:**
    ```bash
    git clone https://github.com/Boon1013/DIG-Macro
    ```
	*or download the .zip and extract it: https://github.com/Boon1013/DIG-Macro/archive/refs/heads/main.zip*
	
3. **Go inside the directory (DIG Macro).**
    
4.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

## How to Run
1.  **Change the in-game settings:**
    * `Minigame Dimming`: **1**

2.  **Change the monitor settings:**
    * `Resolution`: **1920x1080 (16:9)**

3.  **Run the Script:**
    ```bash
    py main.py
    ```
	
4.	**Start the macro:**
	* Press `F7` on your keyboard.

## How to Stop
  * Simply **close the "debug" window**.
  * Alternatively, you can press `Ctrl+C` in the terminal where the script is running.

## Configuration
You can tweak the script's behavior by modifying the settings at the top of the `main.py` file.
| Variable                            | Description                                                                                                         |
| ----------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| `CLICKABLE_WIDTH`                   | Width of the "STRONG" clicking area.                                                                                
| `CHECK_FOR_BLACK_SCREEN`            | Set to `False` to disable the background dimming check (**this will cause a lot of random left clicks**).
| `CLICK_COOLDOWN`                    | Cooldown for debounce in the click handler. (minimizes the missclicks, but makes the macro slower)         
|                                     | 
| `PATHFINDING`                       | Set to `True` to enable pathfinding. (make sure there is space around you - it will try to stay in a small box - **experimental**)         
|                                     | 
| `WINDOW_NAME`                       | Title of the Debug Window.                                                                                          
| `SHOW_DEBUG`                        | Set to `False` to disable the debug window for a slight performance gain (it will open an window with no image instead so you can easily stop the macro).
|                                     | 
| `TOGGLE_KEY`                        | The key that will be used to toggle the macro running (Default is `F7`).
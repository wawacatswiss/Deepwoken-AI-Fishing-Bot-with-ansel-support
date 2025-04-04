# Deepwoken AI Fishing Bot

This bot automatically fishes in the Roblox game *Deepwoken* using a combination of image detection and pixel color detection.

I made this bot as a personal project and never thought i would be releasing it, so I will respond for support but very rarely because i dont even play deepwoken and dont really care about this project anymore. 

**as of 1. of april, this thing still words, also i just look at the fishtrap repo and apperently shaders dont work so this entire repo is useless**

## How It Works
The bot captures the game screen, detects specific in-game UI elements, and performs automated actions (like pressing keys) based on what it sees. It helps to automate the fishing process in the game by identifying the necessary keypresses (A, S, D) during fishing.

## Features
- **Roblox Detection:** Detects the open Roblox window.
- **Key Detection:** Uses image templates to detect which key (A, S, or D) the player needs to press.
- **Automation:** Automatically clicks and holds the necessary key to fish
- **Overlay System:** A colored box that provides visual feedback on the bot's current state.

## Most Recent Update
- added position saving so you dont need to calibrate everytime you open the program
- added new keybind "]" to reset the saved position and calibrate again
- made the boxes transparent to look better
- fixed some bugs regarding player walking off from keys not being released

## Setup
### Prerequisites:
- ONLY WINDOWS 10 TESTED
- Make sure to have *Roblox* open.
- Install dependencies such as `opencv-python`, `pyautogui`, `keyboard`, `numpy`, `psutil`, and `PyQt5`.
- 
- **If the box doesnt fit please use +,= and - to change the size!!!**
- **If the box doesnt fit please use +,= and - to change the size!!!**
- **If the box doesnt fit please use +,= and - to change the size!!!**
- 
- ~~Watch: https://www.youtube.com/watch?v=4a-AFnwOWuo for a visual tutorial~~

### Steps:
1. Open Roblox, then run the bot.
2. A red box will appear on the screen indicating the bot is active but not yet calibrated.
3. **Press "R"** to activate the bot. The box will turn purple, indicating that the bot is in the calibration phase.
4. Cast your fishing rod in the game and allow the bot to detect the needed keys (A, S, D). The calibration phase ensures the bot understands the positions of these keys.
5. Once calibration is complete, the box will turn green, meaning the bot is ready to start fishing automatically.

![](https://github.com/user-attachments/assets/211cbcd7-3cd8-4c3b-aaa4-9093e72b430a)

## Usage
- **Start Fishing:** After calibration, the bot will automatically handle the fishing for you. It detects the key that needs to be pressed and automates the fishing process.
- **Pause/Resume:** You can press "R" at any time to toggle the bot on or off.
- **Reset Saved Positions:** You can press "]" to reset the saved positions file and re-calibrate. -- NEW!!!!!!!
- **Stop:** Closing the program will deactivate the bot.

## Visual Cues:
- **Red Box:** Bot is inactive.
- **Purple Box:** Calibration in progress.
- **Green Box:** Bot is active and ready to fish.

## Important Notes:
- Calibration may be required every time the program starts to ensure the bot can detect the fishing prompts in the game.
- The bot will only work correctly when the correct in-game screen elements are visible and can be captured by the bot so please dont cover the fishing ui ingame.

## How the Code Works
The bot works in three main stages:
1. **Window Detection:** Locates the Roblox window and defines a region for detection.
2. **Calibration:** Captures the in-game key images and matches them against templates (for A, S, D).
3. **Automation:** Automatically presses the detected key, allowing for hands-free fishing.

## Customization:
- You can adjust the sensitivity and thresholds by modifying the `matchThreshold` and time intervals in the code.
- The image templates can be replaced if the in-game UI changes.

## Libraries Used:
- **OpenCV:** For image processing and template matching.
- **PyAutoGUI:** To interact with the screen and perform mouse clicks.
- **Keyboard:** To simulate key presses.
- **NumPy:** For array manipulation and math operations.
- **PSUtil:** To detect and manage the Roblox window.
- **PyQt5:** For creating the on-screen overlay that provides visual feedback.

## Disclaimer:
This bot is intended for educational purposes and personal use only. Use it responsibly and ensure that you adhere to Roblox's terms of service.

Message me on discord for any assistance: **teenypeenyzeeny**

![image (18)](https://github.com/user-attachments/assets/5da77292-b3ba-42bf-97bd-3b303a785836)

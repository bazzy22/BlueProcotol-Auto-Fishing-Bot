# Blue Protocol Star Resonance Fishing Bot
This is a Python-based automation bot designed to automate the fishing minigame in Blue Protocol: Star Resonance. It uses computer vision (OpenCV) and Windows API controls (pywin32) to watch the screen and simulate mouse and keyboard inputs.

### Important Disclaimer
This project is intended for educational purposes only. Using bots or any form of automation may be against the Terms of Service of your game and could result in an account ban. Use this at your own risk.

##  Features
- Auto-Casting: Automatically casts the fishing line at a specified point.

- Bite Detection: Watches for an exclamation mark (!) template to appear, then automatically hooks the fish.

- Minigame Automation:

  - Tension Control: Monitors the color of the tension bar to hold or release the left mouse button, preventing the line from snapping.

  - Directional Control: Detects left and right arrow images, automatically pressing a or d to follow the fish.

- Auto-Re-buy: Detects when the fishing rod slot is empty and automatically opens the map and buys a new rod.

- Auto-Restart: Detects the end of the minigame, clicks the "exit" button, and begins casting again.

## Requirements
- Python 3.x

- The Python packages listed in requirements.txt:

  - numpy

  - opencv-python

  - pywin32

- An assets folder containing the following template images (you must create these yourself by taking screenshots from your game):

  - exclamation_mark.png

  - arrow_left.png

  - arrow_right.png

  - end.png (The "Fish Caught!" or "Exit" button/UI element)

  - fishing_rod_empty.png (The icon indicating no rod is equipped)

## How to Use
- Install Dependencies:
  
"pip install -r requirements.txt"

- Configure main.py:
  
If you don't have a 1920x1080 screen, you have to configure main.py. Check configuration.txt

- Run the Bot:

Open your game and go to your fishing spot.
Run the script from your terminal:

"python main.py"

You will have 3 seconds to click into your game window and make it the active window.

- Stop the Bot:

To stop the bot, switch back to your terminal window and press Ctrl+C.

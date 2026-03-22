# infinite_ammo.py
A Python mod for Resident Evil 6 that provides infinite ammo functionality using REFramework.

## Features

- ✅ Infinite ammo for all weapons
- ✅ Toggle mod on/off in-game
- ✅ Configurable ammo values
- ✅ REFramework integration
- ✅ Easy to customize

## Requirements

- **Resident Evil 6** (PC)
- **REFramework** - [Download here](https://github.com/praydog/REFramework)
- **Python 3.7+**

## Installation

### Step 1: Install REFramework

1. Download REFramework from the [official GitHub repository](https://github.com/praydog/REFramework)
2. Extract the files to your Resident Evil 6 installation directory
3. Run `dinput8.dll` to initialize REFramework

### Step 2: Install the Mod

1. Clone this repository:
   ```bash
   git clone https://github.com/gardeshem12-sys/infinite-ammo-RE6.git
Copy the mod files to your REFramework mods directory:

Code
RE6_Installation/reframework/mods/infinite-ammo-RE6/
Copy infinite_ammo.py to:

Code
RE6_Installation/reframework/mods/infinite-ammo-RE6/infinite_ammo.py
Copy config.json to:

Code
RE6_Installation/reframework/mods/infinite-ammo-RE6/config.json
Step 3: Configuration
Edit config.json to customize the mod:

JSON
{
  "settings": {
    "max_ammo": 9999,        // Maximum ammo value
    "auto_refill": true,     // Automatically refill ammo
    "all_weapons": true,     // Apply to all weapons
    "update_interval": 1     // Update frequency (frames)
  }
}
Usage
In-Game Controls
F1: Toggle infinite ammo on/off
F2: Increase ammo value
F3: Decrease ammo value
Console Commands
The mod provides console commands when REFramework is active:

Code
ammo.toggle      - Toggle infinite ammo
ammo.set 9999    - Set ammo to specific value
ammo.status      - Show current status
File Structure
Code
infinite-ammo-RE6/
├── README.md              # This file
├── config.json            # Mod configuration
├── infinite_ammo.py       # Main mod code
├── LICENSE                # MIT License
└── docs/
    └── DEVELOPMENT.md     # Development guide
How It Works
The mod works by:

Hooking into REFramework's game loop
Scanning for the weapon manager in game memory
Updating ammo values for all weapons every frame
Responding to user input to toggle and configure
Troubleshooting
Mod Not Loading
Ensure REFramework is properly installed
Check that infinite_ammo.py is in the correct directory
Verify config.json is valid JSON
Ammo Not Updating
Make sure the mod is enabled (check console)
Restart the game
Check that Resident Evil 6 is the supported version
Performance Issues
Reduce update_interval in config.json
Disable auto_refill if not needed
Check for conflicting mods
Development
To modify or extend this mod:

Fork this repository
Create a feature branch: git checkout -b feature/my-feature
Make your changes
Test thoroughly in-game
Submit a pull request
See DEVELOPMENT.md for detailed development guide.

License
This project is licensed under the MIT License - see the LICENSE file for details.

Contributing
Contributions are welcome! Please feel free to submit issues or pull requests.

Disclaimer
This mod is provided as-is for educational purposes. Use at your own risk. The author is not responsible for any damage to your game or system. Always back up your game files before using mods.

Credits
REFramework by praydog
Resident Evil 6 by Capcom
Support
For issues, questions, or suggestions, please open an Issue on GitHub.

Last Updated: 2026-03-22

Code
.gitignore

gitignore
# Python
__pycache__/
*.py[cod]
*$py.class
*.so
.Python
build/
develop-eggs/
dist/
downloads/
eggs/
.eggs/
lib/
lib64/
parts/
sdist/
var/
wheels/
*.egg-info/
.installed.cfg
*.egg

# IDE
.vscode/
.idea/
*.swp
*.swo
*~

# OS
.DS_Store
Thumbs.db

# Game/Mod related
*.log
*.tmp

LICENSE

LICENSE
MIT License

Copyright (c) 2026 gardeshem12-sys

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and all copies or substantial portions of the Software
must include the above copyright notice and this permission notice.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
aUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE OR OTHERWISE,
ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
DEALINGS IN THE SOFTWARE.

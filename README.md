# mc-Motion-Games
4 interactive camera-detection games for university open days

## Overview
Control gameplay with hand gestures, body movements, and facial expressions using OpenCV and MediaPipe. Perfect for university open days and events - no controllers needed, just stand and play!

## Games Included
### 🎮 Mario Kart DS - Webcam Edition
Play Mario Kart DS with your hands or phone!  
- Webcam gesture steering  
- 4-player local multiplayer  
- Phone touch controller  
- Based on melonDS fork  

[submodules/mario-cam-kart](submodules/mario-cam-kart)

### 🌀 Jutsu Hand Signs - Naruto Webcam Game
A Naruto-inspired webcam game: choose your ninja and perform hand-sign sequences tracked with MediaPipe!  
- Two powerful Jutsu: Rasengan and Chidori  
- Hand gesture recognition  
- Difficulty levels  
- Naruto characters  

[submodules/jutsu-hand-signs](submodules/jutsu-hand-signs)

## Technology Stack
- **OpenCV** - Computer vision and particle effects
- **MediaPipe** - Hand tracking and gesture recognition
- **Python** - Main application logic
- **melonDS** - Nintendo DS emulator fork

## Installation
```bash
# Initialize submodules
git submodule update --init --recursive

# Install dependencies
pip install -r requirements.txt

# Run the main game or individual submodules
cd submodules/mario-cam-kart && python main.py
# or
cd submodules/jutsu-hand-signs && python main.py
```

## Usage
### Mario Kart DS
1. Open your hand near the camera - tracker locks on
2. Move hand left/right to steer
3. Use phone or keyboard for acceleration/braking
4. Race in local multiplayer!

### Jutsu Hand Signs
1. Select your ninja character
2. Perform the hand-sign sequence shown
3. Complete the pattern to unleash your Jutsu!
4. Watch Rasengan or Chidori erupt on screen!

## License
See LICENSE file for details.

## Acknowledgements
- [melonDS](https://github.com/melonDS-emu/melonDS) - Nintendo DS emulator
- [MediaPipe](https://mediapipe.dev/) - Hand tracking solution
- [OpenCV](https://opencv.org/) - Computer vision library
- Naruto anime series - Inspiration for Jutsu techniques

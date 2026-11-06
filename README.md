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

### 🏒 Hockey-AR - Air Hockey Webcam Game
A high-performance, zero-allocation browser AR air hockey engine controlled entirely via webcam hand tracking!  
- Landmark 9 single-point anchoring and One Euro filtering  
- Sub-frame interpolation and anti-tunneling physics sub-stepping  
- Instant gesture lock and smooth match transition sequence  
- Solo mode and local multiplayer support  

[submodules/hockey-ar](submodules/hockey-ar)

## Technology Stack
- **OpenCV & MediaPipe** - Computer vision, hand tracking, and gesture recognition
- **Python** - Main application logic for Python-based games
- **Vanilla JavaScript & HTML5 Canvas** - Pure browser-native runtime for Hockey-AR

## Installation
```bash
# Initialize submodules
git submodule update --init --recursive

# Install dependencies
pip install -r requirements.txt

# Run Python-based games (Mario Kart or Jutsu Hand Signs)
cd submodules/mario-cam-kart && python main.py
# or
cd submodules/jutsu-hand-signs && python main.py

# Run Hockey-AR (Static browser deployment or local server)
cd submodules/hockey-ar && python -m http.server 8000

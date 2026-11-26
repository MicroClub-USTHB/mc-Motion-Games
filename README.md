<p align="center">
  <img src="./assets/banner.svg" alt="mc-Motion-Games by Micro Club" width="1000" />
</p>

<p align="center">
  <a href="https://github.com/MicroClub-USTHB/mc-Motion-Games/stargazers"><img src="https://img.shields.io/github/stars/MicroClub-USTHB/mc-Motion-Games?style=flat&labelColor=0b0b10" alt="stars" /></a>
  <a href="https://github.com/MicroClub-USTHB/mc-Motion-Games/issues"><img src="https://img.shields.io/github/issues/MicroClub-USTHB/mc-Motion-Games?labelColor=0b0b10" alt="issues" /></a>
  <a href="https://github.com/MicroClub-USTHB/mc-Motion-Games/commits/main"><img src="https://img.shields.io/github/last-commit/MicroClub-USTHB/mc-Motion-Games?labelColor=0b0b10" alt="last commit" /></a>
  <a href="https://github.com/MicroClub-USTHB"><img src="https://img.shields.io/badge/by-Micro%20Club%20USTHB-0b0b10?style=flat" alt="Micro Club USTHB" /></a>
</p>

<p align="center"><a href="#the-games">Games</a> · <a href="#run-them">Run them</a> · <a href="#how-to-play">How to play</a> · <a href="#built-with">Built with</a></p>

---

## Motion Games

Interactive camera-detection games for university open days. Control the game with
hand gestures, body movements and facial expressions using OpenCV and MediaPipe.
No controllers, no setup for the player: walk up, stand in front of the camera, play.

## The games

<table>
<tr>
<td width="50%" valign="top">

### Mario Kart DS, webcam edition

Play Mario Kart DS with your hands or your phone.

- Webcam gesture steering
- Phone touch controller (wheel, buttons or gyroscope)
- Up to 4-player local multiplayer, one window
- A melonDS fork

**[Open the repo](https://github.com/MicroClub-USTHB/mario-cam-kart)** · `submodules/mario-cam-kart`

</td>
<td width="50%" valign="top">

### Jutsu Hand Signs, Naruto webcam game

Choose your ninja and form the hand seals.

- Rasengan and Chidori, drawn live on your hand
- Rule-based hand-sign recognition
- Easy, Medium and Hard
- 1v1 duel in 3D with Three.js

**[Open the repo](https://github.com/MicroClub-USTHB/JutsuHandSigns)** · `submodules/jutsu-hand-signs`

</td>
</tr>
</table>

## Run them

```bash
git clone --recurse-submodules https://github.com/MicroClub-USTHB/mc-Motion-Games.git
cd mc-Motion-Games      # already cloned? git submodule update --init --recursive
```

Each game has its own README with install steps and requirements. Quick start:

```bash
# Jutsu Hand Signs
cd submodules/jutsu-hand-signs && pip install -r requirements.txt && python main.py

# Mario Kart DS (needs your own legally dumped ROM, see its README)
cd submodules/mario-cam-kart && ./play.sh      # play.bat on Windows
```

## How to play

| Game | Steps |
| --- | --- |
| **Mario Kart DS** | Show both hands to the camera and grab an imaginary wheel. Tilt to steer, fist to accelerate, open palm to brake, thumb out for an item. Or scan the QR code and drive from your phone. |
| **Jutsu Hand Signs** | Pick a ninja and difficulty. Form each seal shown on screen and hold it. Finish the sequence and your jutsu erupts on your hand. |

## Built with

| | |
| --- | --- |
| **OpenCV** | camera capture and the particle effects |
| **MediaPipe** | hand tracking and gesture recognition |
| **Python** | game logic |
| **melonDS** | the Nintendo DS emulator the kart game is forked from |

## License and legal

Each game carries its own license, see its repository. Mario Kart DS is an independent fan
project, not affiliated with Nintendo; only play games you own. The Jutsu game is a fan project
inspired by Naruto.

## Acknowledgements

[melonDS](https://github.com/melonDS-emu/melonDS) · [MediaPipe](https://mediapipe.dev/) · [OpenCV](https://opencv.org/)

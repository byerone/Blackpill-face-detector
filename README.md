# Face Song Detector

A fun Python program that plays different songs depending on whose face it detects on your webcam!

## How it works
- When it detects **your face**, it plays your song
- When it detects **someone else's face**, it plays a different song
- When **no face** is detected, the music stops

## Requirements
Install the required libraries:
```bash
pip install opencv-python pygame face-recognition
```

## Setup
Before running the program, add these 3 files to the project folder:

1. **`my_face.jpg`** — A clear, well-lit photo of your face
2. **`your_song.mp3`** — The song that plays when your face is detected
3. **`other_song.mp3`** — The song that plays when someone else's face is detected

## Usage
Run the program:
```bash
python main.py
```
Press **Q** to quit.

## Tips
- Use a clear, front-facing photo with good lighting for the best face recognition accuracy
- If the webcam is laggy, increase `CHECK_EVERY_N_FRAMES` in the config section of the code
- Adjust the volume by changing the value in `pygame.mixer.music.set_volume()` (0.0 to 1.0)

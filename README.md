🐧 Slowed Penguin V2: Retro Vaporwave Studio

A fully functional, browser-based audio workstation designed with a nostalgic 90s OS aesthetic. Slow down your favorite tracks, apply immersive reverb, and watch the visualizer glitch out in real-time.

<img width="1280" height="720" alt="Red Bold News Youtube Thumbnail (1)" src="https://github.com/user-attachments/assets/97668b41-953d-4f3c-a386-f010f4fb170e" />


![linux](https://github.com/user-attachments/assets/acefda4c-8919-4504-8a07-9b73eecc8503)
![win](https://github.com/user-attachments/assets/0c3e4d4e-180f-4627-befc-fd246a520df6)
![mac](https://github.com/user-attachments/assets/80cf7c5c-9c03-444c-8f35-dc7a6bfdd0dc)

✨ Features

Multi-OS Themes: Seamlessly switch between Windows 98, Classic Macintosh, and Caldera Linux environments.

xeyes Integration: Features a functional X11-style xeyes component in the Caldera Linux title bar that tracks your cursor.

Audio Processing: Real-time playback rate (pitch) control, Low-pass filtering, Bass boost, and custom convolution Reverb.

8D Spatializer: Automated stereo panning logic that creates an immersive "moving" audio experience.

Pixel-Mosh Monitor: A CRT-style visualizer utilizing a custom shader-like logic to react to audio frequencies with RGB shifting and glitch effects.

Custom Assets: Drag-and-drop or upload your own audio files and background textures for the monitor.

Session Recording: Built-in MediaRecorder support to capture your visualizer output directly to a .webm video file.

🛠️ Technical Info & DSP Logic

This project leverages the Web Audio API to handle complex signal routing without external libraries:

Sample Rate Manipulation: Uses AudioBufferSourceNode.playbackRate to achieve the "Slowed" effect without the artifacts of standard time-stretching.

Convolution Reverb: Uses a generated impulse response (white noise with exponential decay) processed through a ConvolverNode.

Visualizer Pipeline: The AnalyserNode provides Real-Time Frequency Data (FFT), which is mapped to Canvas manipulation functions to create the "Bass Shake" and "RGB Split" effects.

# Hand Gesture Racing Controller

A real-time hand gesture recognition system that allows users to control racing games using hand movements in front of a webcam.

The project uses **Python, OpenCV, and MediaPipe** to detect and track hand movements, then translates gestures into keyboard inputs for controlling a racing game.

## Features

- Real-time hand tracking using a webcam.
- Detection and tracking of both hands.
- Gesture-based acceleration and braking.
- Steering control through hand orientation.
- Visual feedback with an OpenCV interface.
- Keyboard simulation for compatibility with browser-based racing games.

## Gesture Controls

| Hand Gesture            | Action        |
| ----------------------- | ------------- |
| Two closed fists        | Accelerate    |
| Two open hands          | Brake         |
| Tilt hands to the left  | Steer left    |
| Tilt hands to the right | Steer right   |
| Neutral hand position   | Keep straight |

## Technologies

- **Python 3.11**
- **OpenCV 4.10.0** – Image processing and webcam input.
- **MediaPipe 0.10.21** – Hand detection and tracking.
- **NumPy 1.26.4** – Numerical operations.
- **pynput** – Keyboard input simulation.

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/CongMinhOfficial/Hand-Gesture-Racing-Controller.git
```

### 2. Navigate to the project directory

```bash
cd Hand-Gesture-Racing-Controller
```

### 3. Create a virtual environment

Python 3.11 is recommended.

**Windows:**

```powershell
py -3.11 -m venv .venv
```

Activate the environment:

```powershell
.\.venv\Scripts\Activate.ps1
```

### 4. Install dependencies

```bash
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

## Usage

### 1. Start the application

```bash
python main.py
```

### 2. Position your hands

- Make sure your webcam can clearly see both hands.
- Keep your hands within the camera frame.
- Perform the gestures described in the Gesture Controls section.

### 3. Control the racing game

Open a racing game that supports keyboard controls. The application will translate detected hand gestures into keyboard inputs.

### 4. Exit

Press `Q` or `ESC` to close the application.

## Project Structure

```text
Hand-Gesture-Racing-Controller/
│
├── main.py
├── requirements.txt
├── .gitignore
└── README.md
```

## Requirements

- Python 3.11
- Webcam
- Windows operating system (recommended)
- Racing game with keyboard control support

## Configuration

The application provides configurable parameters in `main.py`, including:

- Camera index
- Steering sensitivity
- Steering dead zone
- Steering release zone

Adjust these values to improve tracking and control according to your webcam and playing environment.

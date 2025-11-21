# Mako G-131C Camera Utilities

This repository contains code utilities designed for interacting with the **Allied Vision Mako G-131C** camera via the Vimba X SDK.

## 📂 Project Structure

```text
├── acquirePictures.py   # Main script for streaming or capturing images
├── listCameras.py       # Utility to find cameras on the network
└── README.md
```

## ⚙️ Prerequisites & Hardware

* **Camera:** Allied Vision Mako G-131C
* **Interface:** GigE (Ethernet) / Local Network
* **Drivers:** Ensure the Vimba X Driver (or Vimba Viewer) is installed and the camera is configured with the correct IP address settings.

## 🛠️ Environment Setup

This project is built using **Python 3.13.7**.

### Dependencies
To run these scripts, you will need the following libraries installed. It is recommended to use a virtual environment.

| Library | Version | Description |
| :--- | :--- | :--- |
| **vmbpy** | `1.1.1` | Allied Vision Python wrapper for Vimba X API |
| **opencv-python** | `4.12` | Used for image processing and display (`cv2`) |

### Installation
You can install the necessary dependencies using pip:

```bash
pip install vmbpy==1.1.1 opencv-python==4.12.0.xx 
# Note: Verify the specific build of opencv-python 4.12 available for your OS
```

---

## 🚀 Usage

### 1. `listCameras.py`
Use this script to verify connectivity. It scans the local network and lists all connected Vimba-compatible cameras.

* **Purpose:** Discovery and connection verification.
* **Command:**
  ```bash
  python listCameras.py
  ```

### 2. `acquirePictures.py`
This script handles image acquisition. It operates in two modes: **Stream** or **Single Picture**.

* **Purpose:** View the camera feed or save an image.
* **Command:**
  ```bash
  python acquirePictures.py
  ```

#### ⚠️ Configuration
To change the operating mode, you must edit the `main` function inside `acquirePictures.py`.

1. Open `acquirePictures.py` in your text editor.
2. Locate the `main()` function.
3. Switch between single picture and streaming mode by calling the function `takePicture()` or `streamPictures()`.

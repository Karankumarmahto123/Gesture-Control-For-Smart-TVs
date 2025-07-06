
# ✋ Gesture Recognition for Smart TV Control

## 📌 Problem Statement

In the era of smart electronics, enhancing user experience through intuitive human-computer interaction is a key goal. This project, initiated by a home electronics company specializing in smart televisions, aims to develop a gesture-based control system that enables users to operate their TVs **without a remote** — using simple hand gestures captured by the built-in webcam.

---

## 🎯 Objective

Build a robust deep learning model that can recognize **five distinct hand gestures** from short video clips (2–3 seconds, 30 frames each). Each gesture corresponds to a specific TV command:

| Gesture        | Command                 |
|----------------|--------------------------|
| 👍 Thumbs Up   | Increase volume          |
| 👎 Thumbs Down | Decrease volume          |
| 👈 Left Swipe  | Rewind 10 seconds        |
| 👉 Right Swipe | Fast forward 10 seconds  |
| ✋ Stop (Palm) | Pause playback           |

---

## 📂 Dataset Structure

The dataset is provided as a `.zip` file containing two main folders:

- `train/`
- `val/`

Each folder contains:

- A set of subfolders with **30 image frames** per video.
- A corresponding `.csv` file with the following columns:
  - `folder_name`: Name of the subfolder containing the gesture frames.
  - `gesture_label`: The gesture as a text label (e.g., `ThumbsUp`, `Stop`).
  - `label`: A numeric class ID (ranging from 0 to 4).

> ⚠️ Videos are recorded in two resolutions: **360×360** and **120×160**. Standardization of image size is required during preprocessing.

---

## ✅ Project Tasks

- [ ] Data preprocessing and frame standardization
- [ ] Gesture label encoding and efficient data pipeline
- [ ] Deep learning model design (e.g., CNNs, 3D CNNs, or CNN + LSTM hybrid)
- [ ] Training and validation on provided dataset
- [ ] Evaluation on unseen validation data
- [ ] Optional: Real-time gesture inference from webcam
- [ ] Performance tuning (accuracy vs latency)

---

## 🛠 Tech Stack

- Python
- OpenCV
- NumPy, Pandas
- TensorFlow / PyTorch
- Matplotlib
- scikit-learn

---

## 🚀 How to Run (To be updated)

1. Clone the repository  
   ```bash
   git clone https://github.com/your-username/gesture-tv-control.git
   cd gesture-tv-control

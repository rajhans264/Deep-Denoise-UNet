# 🎧 SpectralClean: Deep Learning Speech Enhancement (U-Net)

A robust AI-powered solution to remove stationary background noise (Blower/Fan noise) from speech signals using a U-Net architecture. Developed as part of a high-accuracy signal processing assignment.

---

## 🚀 Overview
This project utilizes a **Convolutional Autoencoder (U-Net)** to perform speech enhancement. By converting raw audio into **Log-Magnitude Spectrograms**, the model learns to isolate speech patterns from continuous blower noise, achieving a reconstruction accuracy of **≥ 95%**.

### 📊 Performance Metrics
- **Target Accuracy:** 95% (Measured via MAE < 0.05)
- **Architecture:** U-Net with Skip Connections (to preserve vocal harmonics)
- **Domain:** Frequency-domain processing (STFT)

---

## 🛠️ Tech Stack
* **Language:** Python 3.12+
* **Framework:** TensorFlow / Keras
* **Signal Processing:** Librosa, SoundFile, SciPy
* **Visualization:** Matplotlib

---

## 📈 Visualizations Generated
The script produces three critical plots for evaluation:
1. **Epochs vs. Error:** Monitors the loss convergence to prove the 95% accuracy threshold.
2. **Time-Domain Waveform:** Side-by-side comparison of the noisy input vs. the cleaned output.
3. **Spectral Heatmap:** Spectrogram analysis showing the removal of low-frequency blower noise.

---

## 💻 Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/SpectralClean-UNet.git](https://github.com/your-username/SpectralClean-UNet.git)
   cd SpectralClean-UNet
2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
3. **Usage:**
   Ensure clean_speech.wav and blower_noise.wav are in the root directory.
   
## 📁 Project Structure
├── main.py                # Core Logic (Training + Inference + Plotting)
├── requirements.txt       # Library dependencies
├── README.md              # Documentation
├── clean_speech.wav       # Clean speech data
└── blower_noise.wav       # Blower noise sample

## 🎓 Academic Context
This project was developed for a professional AI submission. It demonstrates advanced concepts in System Design for audio processing, focusing on real-world noise suppression for educational coaching content.

The implementation highlights:
 -Feature Engineering: Log-Magnitude STFT conversion.
 -Architecture: U-Net Autoencoder with Skip Connections.
 -Evaluation: Mathematical convergence of Mean Absolute Error (MAE) to achieve ≥ 95% reconstruction accuracy.
Author: Rajhans Jain
Location: Jabalpur, MP

# ECG-Bio-Signal-Analyzer# 🫀 ECG Bio-Signal Analyzer

An advanced MATLAB desktop graphical user interface (GUI) developed for biomedical signal processing, filtering, feature extraction, and machine learning classification of Electrocardiogram (ECG) signals.

---

## 🚀 Features & Architecture

* **Multi-Tab Workspace**: Includes 7 distinct interactive analytical views:
  1. **Time Domain**: Visualizes raw noise-corrupted signals, filtered signals, resampled signals ($250\,\text{Hz}$), and automated **R-Peak detection**.
  2. **Frequency Domain**: Computes FFT magnitude spectra for both raw and filtered signals across full and ECG-specific bands ($0\text{--}40\,\text{Hz}$).
  3. **Spectrograms**: Short-Time Fourier Transform (STFT) time-frequency representations and Heart Rate Variability (HRV) analysis.
  4. **Filter Design**: Interactive IIR filter designer supporting Butterworth and Chebyshev Type I implementations (Bandpass $0.5\text{--}150\,\text{Hz}$, Notch $50\,\text{Hz}$) with real-time Pole-Zero mapping, impulse response, and phase/magnitude plots.
  5. **Feature Extraction**: Automatically computes 11 distinct biomedical features (Mean, Median, Variance, RMS, Dominant Frequency, Band Power, Heart Rate, SNR, Skewness, Kurtosis, Zero-Crossing Rate).
  6. **Machine Learning / AI**: Auto-trains classifiers (SVM, KNN, Decision Tree, Random Forest, Naive Bayes) using augmented datasets and classifies incoming signals with confusion matrices and feature importance metrics.
  7. **Signal Comparison**: Cross-compares a secondary loaded signal against the primary reference signal using Euclidean distance and similarity scoring.

---

## 🛠️ Requirements & Setup

* **Software**: MATLAB (R2022a or newer recommended) with the following toolboxes:
  * Signal Processing Toolbox
  * Statistics and Machine Learning Toolbox
* **Execution**: Open MATLAB, navigate to the project directory, and run the main script:
  ```matlab
  ECG_GUI_Final1

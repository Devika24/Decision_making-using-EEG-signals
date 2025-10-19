# Decision-Making Analysis Using EEG Signals

This project investigates **human decision-making patterns** using EEG (Electroencephalography) signals.  
It explores how different brain regions synchronize during decision tasks, using frequency-domain features, correlation analysis, and clustering methods.

---

## 🧩 Overview

The notebook `Decision_making_with_eeg_dataset_updated.ipynb` performs:
1. **Data Loading** – Reads `.set` EEG files using MNE and extracts six key electrodes:
   - **Occipital:** O1, O2  
   - **Parietal:** P7, P8  
   - **Prefrontal:** FP1, FP2  

2. **Signal Processing** – Applies Fast Fourier Transform (FFT) and selects frequency bands (Alpha, Beta, Theta, Gamma) for analysis.

3. **Feature Extraction** – Builds **region-level features** by combining left/right channel magnitudes within each brain region.

4. **Cross-Subject Correlation** – Computes **Pearson** and **Spearman** correlations between subjects to measure inter-brain synchrony.

5. **Clustering** – Uses **K-Means** to group subjects with similar neural decision-making signatures.

6. **Visualization** – Plots frequency spectra, correlation heatmaps, and clustering patterns.

---

## 🧠 Research Goal

To uncover **neural synchronization patterns** during decision-making tasks and compare:
- **Occipital** (visual processing),
- **Parietal** (integration and attention),
- **Prefrontal** (executive and control) regions.

---

## ⚙️ Technologies Used

| Category | Tools |
|-----------|-------|
| EEG Processing | MNE, SciPy, NumPy |
| Data Handling | Pandas |
| Visualization | Matplotlib, Seaborn |
| Modeling | scikit-learn (KMeans, Correlation) |
| Experimental DL | TensorFlow / Keras (Siamese & CNN prototypes) |

---

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/Devika24/Decision_making-using-EEG-signals.git
   cd Decision_making-using-EEG-signals

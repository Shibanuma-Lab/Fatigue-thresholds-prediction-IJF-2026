# Fatigue thresholds prediction-IJF-2026

### `fatigue-thresholds-prediction-model/` (Threshold Prediction Framework)
- **Purpose**: Corresponds to **Sections 4 and 5** of the manuscript. It implements the threshold prediction framework on an idealized semi-infinite body. 
- **Contents**:
  - **Forward Analysis Script** (`forward_analysis.py`): Calculates the fatigue life analytically to generate the reference S-N curve (failure probability) and determine the reference applied stress amplitude ($\sigma_{\mathrm{ref}}$).
  - **Inverse Analysis Script** (`fatigue_thresholds_prediction.py`): Implements the crack arrest condition (da/dN=0) to determine the critical driving force. It generates the Kitagawa–Takahashi (K-T) diagram and cyclic R-curve for identifying four key parameters: $\sigma_{\mathrm{e}}$, $\Delta K_{\mathrm{th,LC}}$, $d_1$, and $d_2$.
  - Microstructural information.
- **Usage**: Run the forward analysis script first to obtain the reference stress, followed by the inverse analysis script to predict the thresholds.

## Requirements
- Python 3.x
- Required libraries: `numpy`, `pandas`, `scipy`

Install the dependencies using:
```bash
pip install numpy pandas scipy

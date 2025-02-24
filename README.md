# Voice Activity Detection (VAD) - Homework

## Overview
This lab implements and evaluates Voice Activity Detection (VAD) using two different approaches:

1. **Energy-Based Approach**: Detects speech based on short-term energy analysis.
2. **K-Means Clustering Approach**: Uses unsupervised learning to classify speech and silence frames.

## Implementation Details
- The **energy-based method** applies a bandpass filter, computes short-term energy, and detects speech by setting an adaptive noise threshold.
- The **K-Means method** clusters audio frames based on extracted features to classify speech vs. non-speech segments.
- The detection results are compared using a detection error rate (DER) metric.

## Results
| Approach                 | Detection Error Rate (DER) |
|--------------------------|---------------------------|
| Energy-Based Approach   | 12.6%                     |
| K-Means Approach       | 33.4%                     |

## Usage
To run the notebook:
1. Install dependencies:  
   ```bash
   pip install kaggle numpy pandas matplotlib librosa soundfile pyloudnorm scipy scikit-learn ipywidgets torch pyannote.audio mir_eval
   ```
2. Execute the Jupyter Notebook step by step.
3. Modify parameters if needed and analyze results.


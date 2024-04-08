
# Lab 7

Speech Feature Extraction and HMM Classification

## Learnings
- This lab explored using Hidden Markov Models (HMMs) for speech signal classification.
- Focused on feature extraction using Short-Time Fourier Transform (STFT) to represent speech in a time-frequency domain.
The lab aimed to set up the groundwork for HMM classification (not implemented here due to its complexity).

## Lab Tasks
1. STFT Feature Extraction:

- Loaded recorded speech signal from Lab 2.
- Employed `librosa.stft` to compute the STFT representation of the signal.
- Obtained a time-frequency representation where each element reflects the spectral magnitude at a specific time and frequency bin.
(Optional: Explore different parameters for STFT like window size and hop length to understand their impact on feature resolution)
## Further Exploration

 - Implement a basic HMM for speech classification using extracted STFT features (advanced).
- Investigate feature extraction techniques like Mel-Frequency Cepstral Coefficients (MFCCs) for improved speech recognition performance.
- Explore applications of HMM-based speech recognition systems for tasks like keyword spotting or speaker identification.
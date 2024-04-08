
# Lab 5

Spectral Filtering of Speech Signals


## Learnings
- This lab explored filtering speech signals in the frequency domain by manipulating their spectrums.
- Used rectangular windows to select specific frequency bands (low-pass, band-pass, high-pass) and reconstructed the signals for audio playback.
- Investigated the impact of different filter types (rectangular, cosine, Gaussian) on the filtered sounds.

## Lab Tasks
1. Spectral Filtering with Rectangular Windows:

- Performed FFT on the recorded speech signal to obtain its frequency spectrum.
- Used rectangular windows to isolate specific frequency regions:
    * Low-pass filter: Selected only the low-frequency components.
    * Band-pass filter: Selected a desired band of frequencies.
    * High-pass filter: Selected only the high-frequency components.
- Inverted the filtered spectrums using IFFT to reconstruct the time-domain signals.
- Played back the filtered signals to observe the effect on the original speech sound.
2. Comparison of Filter Types:

- Repeated spectral filtering using different window functions:
    - Cosine window
    - Gaussian window
- Compared the reconstructed sounds obtained with each filter type.
- Analyzed how different window shapes affect the filtering characteristics (e.g., sharpness of transitions between frequency bands).
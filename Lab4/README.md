
# Lab 4

Speech Signal Analysis in Frequency Domain


## Learnings
- This lab explored techniques for analyzing speech signals in the frequency domain using Fourier transforms.
- Implemented the Fast Fourier Transform (FFT) to convert speech signals from the time domain to the frequency domain.
- Analyzed the spectral content of speech signals and compared full signal vs. individual word spectrums.
- Investigated windowing effects on spectral analysis using Short-Time Fourier Transform (STFT).
- Visualized the time-frequency representation of speech using spectrograms.

## Lab Tasks
1. Speech Signal to Frequency Domain:

- Used `numpy.fft.fft` to compute the Discrete Fourier Transform (DFT) of the recorded speech signal.
- Plotted the magnitude (amplitude) of the spectral components to observe the frequency distribution.

2. Inverse Transform:

- Employed `numpy.fft.ifft` to perform the inverse DFT, converting the frequency spectrum back to the time domain.
- Compared the reconstructed signal with the original speech signal to evaluate potential distortions.

3. Word vs. Full Signal Spectrum:

- Identified a specific word within the recorded speech.
- Computed and compared the frequency spectrum of the word with the spectrum of the entire signal.
- Analyzed how the spectral content differs between a single word and the whole utterance.

4. Windowed FFT Analysis:

- Defined a rectangular window of 20 milliseconds at a sampling rate of 22.5 kHz.
- Used FFT to analyze the spectral components of the windowed speech segment.
- Observed how windowing affects the frequency resolution.

5. Short-Time Fourier Transform (STFT):

- Segmented the speech signal into short windows (20 milliseconds) with some overlap.
- Employed `numpy.fft.rfft` to compute the real-valued FFT for each window, obtaining frequency components.
- Stacked these frequency components as columns to form a time-frequency representation matrix.
- Visualized the matrix as a heatmap to display the spectral variation over time.
(Alternatively, use `librosa.stft` or `scipy.signal.stft` for STFT computation)

6. Spectrogram Analysis:

- Utilized scipy.signal.spectrogram to generate a spectrogram of the speech signal.
- Compared the spectrogram visualization with the heatmap from the STFT analysis.
- Observed how spectrograms provide a more intuitive representation of time-frequency variations in speech.
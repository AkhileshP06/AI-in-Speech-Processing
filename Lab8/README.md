
# Lab 8

Speech Recognition with Deep Learning and Phoneme-based Synthesis

## Learnings
- This lab explored Deep Learning architectures like LSTMs and Bi-LSTMs for speech recognition tasks.
- Reviewed feature extraction techniques (STFT, MFCC, LPC) for representing speech signals.
- Investigated phoneme-based speech synthesis and its limitations.
## Lab Tasks
1. Speech Recognition with Deep Learning:

- Explored using pre-trained models or tutorials for building LSTMs or Bi-LSTMs for speech recognition.
- Focused on understanding the model architecture, training process, and evaluation metrics for speech recognition.

2. Phoneme-based Speech Synthesis:

- Extracted MFCC features from the recorded sentence "Bhanumathi weds Rajat". (You can replace MFCC with other features like STFT or LPC)
- Segmented the sentence into phonemes using a pre-trained phoneme recognizer or manual labeling.
- Concatenated phonemes from the segmented speech (e.g., using phonemes from "Bhanumathi" to synthesize "Bharat") to create a new word.
- Played back the synthesized word "Bharat" and observed the quality compared to natural speech.
## Further Exploration

- Train your own LSTMs or Bi-LSTMs for speech recognition on a larger speech dataset (advanced).
- Investigate Deep Neural Networks (DNNs) or Convolutional Neural Networks (CNNs) for speech recognition.
- Explore more sophisticated speech synthesis techniques like WaveNet or mel-spectrogram inversion for generating high-quality synthetic speech.
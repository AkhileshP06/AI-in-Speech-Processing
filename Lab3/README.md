
# Lab 3

Speech Segmentation


## Learnings
- This lab explored functionalities in librosa for speech segmentation.
- We used `librosa.effects.trim` to remove silence from the beginning and end of speech signals.
- We investigated `librosa.effects.split` for segmenting speech based on detected silence intervals.
- Compared the performance of librosa's silence detection with an external method from the provided reference.

## Lab Tasks
1.Silence Removal: 
- Used `librosa.effects.trim` to remove leading and trailing silence from the recorded speech signal (Lab 2).
- Listened to the trimmed signal and compared its audio quality with the original.
2. Speech Splitting:

- Employed `librosa.effects.split` to segment the recorded speech based on detected silence intervals.
- Experimented with the `top_db` parameter to adjust sensitivity for silence detection.
- Analyzed the generated segments and observed the quality of the split.
3. External Silence Detection Comparison:

- Reviewed the provided IEEE paper on silence detection methods.
- Compared the silence detection results obtained from librosa with the method described in the paper.
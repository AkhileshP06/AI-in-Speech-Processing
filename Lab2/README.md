
# Lab 2

First Derivative, Zero Crossings

## Learnings
- This lab explored the finite difference method for approximating the first derivative of a speech signal.
- Analyzed zero-crossing points in the derivative to identify potential speech and silence regions.
- Compared the lengths of spoken words and investigated the impact of intonation on speech signal characteristics.

## Lab Tasks
1. Speech Signal Derivative: Calculated the first derivative of the recorded speech signal from Lab 1 using the finite difference method.
```python
  def finite_difference(signal, sampling_rate):
    dt = 1.0 / sampling_rate
    derivative = np.diff(signal) / dt
    return np.concatenate(([0], derivative))
```
2. Zero-Crossing Detection: Identified points where the derivative signal crosses the zero axis (zero-crossings).
```python
def zero_crossings(derivative):
    return np.where(np.diff(np.sign(derivative)))[0]
```
3. Speech vs. Silence Analysis: Compared the average length between consecutive zero crossings in speech and silence regions.
```python
def calculate_average_length(zero_crossings):
    return np.mean(np.diff(zero_crossings))
```
4. Word Length Comparison: Recorded five favorite words and analyzed their signal lengths. Compared these lengths with a [@D Subham's](https://github.com/Subham-Dwarapu) recordings.

5. Statement vs. Question: Recorded a sentence spoken as both a statement and a question. Analyzed and compared the two speech signals.
```python
plt.figure(figsize=(10, 6))
plt.plot(time_axis, yk1, color='blue', label='Audio 1')
plt.plot(time_axis, yk2, color='red', label='Audio 2')
plt.title('Comparison of Audio Signals')
plt.xlabel('Time (seconds)')
plt.ylabel('Amplitude')
plt.legend()
plt.grid(True)
plt.show()
```
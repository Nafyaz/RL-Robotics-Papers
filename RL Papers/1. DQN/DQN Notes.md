Link: https://web.stanford.edu/class/psych209/Readings/MnihEtAlHassibis15NatureControlDeepRL.pdf
### Abstract
- Previously RL was limited to domains where features can be handcrafted, or in domains with fully observed low dimensional state spaces.
- Introduces deep neural network (Deep Q Network) that learns policies directly from high-dimensional sensory inputs.
- Tested in 49 Atari 2600 games using same algorithm, network architecture and hyper-parameters.

### Introduction
- [x] Use CNN
- Minimize Action value function
- RL can be unstable or sometimes diverge. 
	- Reason 1: Correlations in the sequence of observations. Therefore, introducing experience replay.
	- Reason 2: Correlation between action values and target values. Therefore, iterative update action values and periodically update target values.
### Methodology
Preprocessing:
1. Some objects flicker (i.e. appear in one frame, disappears from next). Take max value of each color from this frame and the previous one.
2. Take only Y channel (luminance) from RGB
3. Rescale frames from 210x160 pixels with 128 color palette to 84x84.
4. Stack m=4 most recent frames in order to get a state. m=3, or 5 works too.

Model:
1. Input: 84x84x4
2. First hidden layer: 32 filters of 8x8 with stride 4. ReLU
3. Second hidden layer: 64 filters of 4x4 with stride 2. ReLU
4. Third hidden layer: 64 filters of 3x3 with stride 1. ReLU
5. Final hidden layer: fully connected 512 rectifier units.
6. Output layer: Number of valid actions.

![[Pasted image 20251009172753.png|775]]

### Results

![[Pasted image 20251013000252.png]]

![[Pasted image 20251013001217.png]]
![[Pasted image 20251013001417.png]]
### Discussions

### Conclusion

### References

Link: https://web.stanford.edu/class/psych209/Readings/MnihEtAlHassibis15NatureControlDeepRL.pdf
### Abstract

- Previously RL was limited to domains where features can be handcrafted, or in domains with fully observed low dimensional state spaces.
- Introduces deep neural network (Deep Q Network) that learns policies directly from high-dimensional sensory inputs.
- Tested in 49 Atari 2600 games using same algorithm, network architecture and hyper-parameters.

### Introduction
- Use CNN
- Minimize Action value function
- RL is unstable or sometimes diverge. 
	- Reason 1: Correlations in the sequence of observations. Therefore, introducing experience replay.
	- Reason 2: Correlation between action values and target values. Therefore, iterative update action values and periodically update target values.
### Methodology

![[Pasted image 20251009172753.png|775]]

### Results

![[Pasted image 20251013000252.png]]

![[Pasted image 20251013001217.png]]
![[Pasted image 20251013001417.png]]
### Discussions

### Conclusion

### References

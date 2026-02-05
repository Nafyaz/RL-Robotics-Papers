1. DQN paper's experience replay uniform-randomly selects samples
2. But what if the target is moving and old samples become obsolete with time?
3. So, we can introduce a replay buffer that gives more weight to later samples and less to earlier ones.
4. Can we save replay buffers in neural nets?
5. Using two NNs: NN for target value, NN for action value because their might be correlation between them. Isn't it obvious?? I didn't understand this part. Gemini says "dog chasing its tail" problem. What does it mean?!
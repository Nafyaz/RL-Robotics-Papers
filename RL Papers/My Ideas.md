1. What about weighted replay buffers?
	- DQN paper's experience replay uniform-randomly selects samples
	- But what if the target is moving and old samples become obsolete with time?
	- So, we can introduce a replay buffer that gives more weight to later samples and less to earlier ones.
	- Can we save replay buffers in neural nets?
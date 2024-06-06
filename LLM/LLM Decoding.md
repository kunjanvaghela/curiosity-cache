
 Decoding is the process of generating text with an LLM.
- Iterative process, one word at a time.

### How to pick a word?
1. Greedy Decoding:
	- Pick the highest probability word at each step.
	- Simplest
2. Non-Deterministic Decoding:
	- Pick randomly among the high probability candidates at each step.
	- **Temperature:**
		- A hyper parameter that modulates the distribution over vocabulary.
		- *Temperature Decreased*: Distribution is peaked around the most likely word.
		- *Temperature Increased*: Distribution is flattened over all words.
	- **Top_p**: Get from top p%.

### Most common types:
1. Greedy
2. Nucleus Sampling - Similar to Non-Deterministic but has few additional parameters which govern specifically which portion of words to sample from.
3. Beam Search - Where multiple sequences are generated simultaneously and continually prune the sequences with low probability.

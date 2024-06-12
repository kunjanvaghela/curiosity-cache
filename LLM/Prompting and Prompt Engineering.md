
### Prompt:

- Text provided to an LLM as input, may contain instructions or/and examples.
- To change the prompt is the simplest way to affect the distribution over the vocabulary.

### Prompt Engineering:

- Process of iteratively refining a prompt for the purpose of eliciting a particular style of response.

### Strategies for Prompting:

##### 1. In-context learning:
  - Prompting an LLM with instructions and/or demonstrations of the task it is meant to complete.
  - Few shots/k-shot prompting:
	  - Explicitly providing k examples of the intended task in the prompt.
##### 2. Chain-of-thought prompting:
  - Prompt the LLM to emit intermediate reasoning steps.
##### 3. Least-to-most prompting:
  - Prompt the LLM to decompose the problem and solve, easy-first.
##### 4. Step-back:
  - Prompt the LLM to identify the high-level concepts pertinent to a specific task.

## Issues with Prompting

### Prompt Injection (jailbreaking):

- To deliberately provide input to LLM that attempts to cause it to ignore instructions, cause harm, or behave contrary to deployment expectations.
- Note: Prompt Injection is a concern any time an external entity is given the ability to contribute to the prompt.





## Prompt Engineering
- Reinforcement Learning from Human Feedback (RLHF)
	- is used to fine-tune LLMs to follow a broad class of written instructions.
- Prompt Formats
	- LLMs are trained on a specific format. Different format prompts may get odd/inferior results.
	- For example: Llama2 is fine tuned for instruction tags, if not provided, it may generate different output than expected.

- Budding area of research where LLM-based agents
- For sequential decision making scenarios, for ex. playing chess, operating s/w autonomously, or in searching a product in the web expressed in NLP.

### Idea
- In its environment, iteratively takes actions to accomplish a specific goal.
- Model observes results and keeps on taking action within its environment till goal is accomplished.

### Notable Work
1. [ReAct](https://arxiv.org/pdf/2403.14589) : Iterative framework where LLM emits thoughts, then acts, and observes result.
2. [Toolformer](https://arxiv.org/pdf/2302.04761): Pre-training technique where strings are replaced with API calls to tools that yield result.  
3. [Bootstrapped Reasoning](https://arxiv.org/pdf/2203.14465): Prompt the LLM to emit rationalization of intermediate steps; use as fine-tuning data.
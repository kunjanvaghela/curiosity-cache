
LangChain is a framework for developing applications powered by large language models (LLMs).


Concretely, the framework consists of the following open-source libraries:

1. langchain-core: Base abstractions and LangChain Expression Language.
2. langchain-community: Third party integrations.
3. Partner packages (e.g. langchain-openai, langchain-anthropic, etc.): Some integrations have been further split into their own lightweight packages that only depend on langchain-core.
4. langchain: Chains, agents, and retrieval strategies that make up an application's cognitive architecture.
5. LangGraph: Build robust and stateful multi-actor applications with LLMs by modeling steps as edges and nodes in a graph. Integrates smoothly with LangChain, but can be used without it.
6. LangServe: Deploy LangChain chains as REST APIs.
7. LangSmith: A developer platform that lets you debug, test, evaluate, and monitor LLM applications.



## LangChain Components:

1. LLMs
2. Prompts
3. Memory
4. Chains
5. Vector Stores
6. Document Loaders



### 2. Prompt Templates

- Prompt templates are predefined recipes for generating prompts for language models.
- Typically, prompt are either a string or else a list of chat messages.
- Types:

##### String Prompt Template:

This supports any number of variables, including no variables.
Example:

```python

prompt_template = PromptTemplate.from_template("Tell me a {adjective} joke about {content}.")
```


##### Chat Prompt Template:

The prompt to chat models is a list of chat messages. Each chat message is associated with content, and an additional parameter called role.
Example:

```python

chat_template = ChatPromptTemplate.from_messages(
	[
		("human", "Hellow, how are you doing?"),
		("ai", "I am doing well, thanks!")
])
```



### 3. LangChain Memory

- Ability to store info about past interactions.
- Chain interacts with the memory twice in a run:
	1. Read from Memory: After user input and before chain execution.
	2. Write to memory: After core logic, before output.
- Challenges:
	- Multiple Users: Need to maintain different chat history, can be done using sessions (ex by using Streamlit).


### 4. LangChain Chains

- Using LCEL (LangChain Expression Language)
```python

llm = OCIGenAI()
prompt = ChatPromptTemplate.from_messages([("",""), ("","")])

runnable = prompt | llm | StrOutputParser()
response = runnable.invoke({"question" : "Some question"})
print(response)
```


- Legacy - Create chains using Python classes like LLM Chain and others.

```python

chain = LLMChain(
		llm=llm,
		prompt=prompt,
		output_parser = StrOutputParser()
	)

response = chain.invoke({"question" : "Some question"})
print(response)
```



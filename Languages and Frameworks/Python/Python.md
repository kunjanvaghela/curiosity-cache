

[[Django]]

## Python Inner Working

- Running a python file:
	- `.py` --> Byte Code (mostly hidden) --> Virtual Machine
- ByteCode:
	- `.pyc` – compiled Python (frozen binaries)
	- `__pycache__` - .pyc is inside this folder
	- Not a machine code, python specific interpretation.
- Python Virtual Machine (PVM) – aka python interpreter
	- Code loop to iterate byte code
	- Run time engine

## Immutable vs Mutable

- Mutable: data can be changed at the allocated memory.
- Immutable: data cannot be changed at the allocated memory.

## Memory Allocation

- Different variables having the same value can be pointed internally to the same memory address (containing the value). --> Maintained by **reference count**.
- Python hides reference count by default, hard to check, however there is a function: `sys.getrefcount(<value>)`.
- Garbage Collection:
	- Managed internally.
	- No immediate garbage collection for Integer and String values: This are usually not cleared soon to have new references later upon allocation.
- `<var1> is <var2>` --> Used to check if memory allocated is same.

## Iter tool
- Use of built-in method next() or __next__() to go to the next element.
- StopIteration exception encountered when the iteration is completed.

#### Function
- `*args` --> For different variable arguments
- `**kwargs` --> For different key-value pair arguments

## Generator with Yield

## Scopes and Closures

- Scope is checked iteratively of the last parent until the variable can be found.
- Global --> the global scope of the program
- Closure --> Whenever a function is returned, it returns localized references as well as per the given function.

#### Class

- For inherited class:
	- `super().<parent class method>`
- Private variables/functions: `use name as __<name>`
- Static method use:
	- `@staticmethod`
- Check if instance of: `isinstance(<instance_name>, <object_name>)`

- Dunder methods: `__<function_name>__()` --> Ex. `__main__()`, `__init__()`
- Private methods (intended, but not enforced by Python): `_<attributename>`
- Name Mangling: `__<attributename>` --> Used for specifically class only.



## Performance Optimization

#### Identifying the bottleneck
1. Using timers - time
2. Using cProfile
3. Using LineProfiler

#### Ways
1. Use in built-functions & compiled libraries (like NumPy, Pandas, Pillow):
	1. This functions are written in C, hence are faster
2. Using Generators when working with massive data
	1. Can reduce memory allocations --> Increasing performance
3. Concurrency
	1. Multiprocessing
	2. Multithreading
	3. Coroutines
4. Compiling with Cython
5. Using PyPy interpreter
	1. Uses JIT interpretation. 
	2. Checks the code before and compiles it beforehand
6. Memoization/Caching at function level
	- Decorator based caching
7. as


## Good Habits

1. Use main() in combination with the following:
```python
def funca():
	pass

def main():
	funca()
	# Some operations

if __name__ == '__main__':
	main()

```
2. Avoid big functions
3. Use type annotations to make python to have data types in introducing variables.
	- mypy module --> performs static type checker
4. Using list comprehensions



## Questions:

Q. Implement decorator with parameters
A.
```python
def decorator_with_args(decorator_arg1, decorator_arg2):
    def actual_decorator(func):
        def wrapper(*args, **kwargs):
            print(f"Decorator arguments: {decorator_arg1}, {decorator_arg2}")
            return func(*args, **kwargs)
        return wrapper
    return actual_decorator

@decorator_with_args("Hello", "World")
def say_hello():
    print("Hello!")

say_hello()

```

Q. Write Dict comprehension
A. 
```python
# Example: creating a dictionary where keys are numbers and values are their squares
squares = {num: num**2 for num in range(10)}
print(squares)

```


Q. Swap Dict keys and values AWS questions
A.
```python
# Example dictionary
original_dict = {'a': 1, 'b': 2, 'c': 3}

# Swapping keys and values
swapped_dict = {v: k for k, v in original_dict.items()}
print(swapped_dict)

```

Q. What is pd.series
A. `pd.Series` is a one-dimensional array-like object in pandas that can hold data of any type (integers, strings, floating point numbers, etc.). It is similar to a column in a DataFrame. Each element in a `Series` has an index, which can be used to access the elements.

Q. What is `__slots__`?
A. `__slots__` is a mechanism in Python that allows you to explicitly declare data members (like attributes) and prevent the creation of `__dict__` and `__weakref__` for instances of the class. This can save memory and speed up attribute access.

Q. What are meta classes?
A. Metaclasses are the 'classes of classes' in Python. They define the behavior of classes and can be used to modify class creation, for instance, to enforce certain constraints or to automatically register classes. The default metaclass in Python is `type`.

Q. Describe how does OAuth 2.0 works?
A. OAuth 2.0 is an authorization framework that allows applications to obtain limited access to user accounts on an HTTP service. It works by allowing the user to authorize an application to access their data without sharing their credentials. The flow typically involves:

1. The client requests authorization from the resource owner.
2. The resource owner provides authorization.
3. The client receives an authorization grant.
4. The client uses the authorization grant to request an access token from the authorization server.
5. The authorization server issues an access token.
6. The client uses the access token to access protected resources from the resource server.


Q. What is circular buffer?
A. A circular buffer, or ring buffer, is a fixed-size buffer that wraps around upon reaching its end. It uses two pointers, a read and a write pointer, which are incremented as data is read from and written to the buffer. When the end of the buffer is reached, the pointers wrap around to the beginning, making efficient use of memory.

Q. Difference between Floyd Warshall, Krushal and Page Rank algorithms?
A.
- **Floyd-Warshall**: An algorithm for finding shortest paths in a weighted graph with positive or negative edge weights. It computes shortest paths between all pairs of nodes.
- **Kruskal's**: An algorithm for finding the minimum spanning tree of a graph. It sorts all the edges in the graph and adds them one by one to the spanning tree, ensuring no cycles are formed.
- **PageRank**: An algorithm used by Google Search to rank web pages in their search engine results. It measures the importance of web pages by considering the number and quality of links to each page.


Q. What is the mechanism for data exchange in distributed system? What is RPC?
A. The mechanism for data exchange in distributed systems often involves message passing or shared memory. RPC (Remote Procedure Call) is a protocol that allows a program to execute a procedure on a remote server as if it were a local call, abstracting the complexities of network communication.

Q. What is pre fetch file blocks based on predicted access patterns?
A. Prefetching file blocks based on predicted access patterns involves anticipating the data blocks that will be accessed in the near future and loading them into memory in advance. This reduces the wait time for data access and improves performance.

Q. NFA vs DFA? Mini Algorithm?
A.
- **NFA (Nondeterministic Finite Automaton)**: A finite state machine where for some cases, a symbol can lead to multiple states. It allows for multiple transitions for a single input symbol.
- **DFA (Deterministic Finite Automaton)**: A finite state machine where each state has exactly one transition for each possible input. It is simpler and more efficient than NFA but less flexible.

Mini Algorithm to convert NFA to DFA:

1. Start with the initial state of the NFA and create an initial state for the DFA.
2. For each state in the DFA, compute its possible transitions by considering all possible states in the NFA.
3. If a new set of states is found, create a new DFA state.
4. Repeat until all states and transitions are processed.


Q. Define analysis of function call times and identify performance bottlesnecks in Python
A. To analyze function call times and identify performance bottlenecks in Python, you can use the `cProfile` module:
```python
import cProfile
import pstats
import io

def some_function():
    # function implementation
    pass

# Profile the function
profiler = cProfile.Profile()
profiler.enable()
some_function()
profiler.disable()

# Output the profiling results
s = io.StringIO()
ps = pstats.Stats(profiler, stream=s).sort_stats('cumulative')
ps.print_stats()
print(s.getvalue())
```
This will give you a detailed report of the time spent in each function, helping you identify bottlenecks.


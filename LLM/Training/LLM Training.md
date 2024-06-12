- For Domain-Adaptation

| Training Style                             | Modifies            | Data                   | Summary                   | Notes                                                                                        |
| ------------------------------------------ | ------------------- | ---------------------- | ------------------------- | -------------------------------------------------------------------------------------------- |
| [[Fine-Tuning (FT]])                       | All parameters      | Labeled, task-specific | Classic ML training       | Full fine tuning an already existing model like BERT                                         |
| [[Parameter Efficient Fine Tuning (PEFT)]] | Few, new parameters | Labeled, task-specific | + Learnable params to LLM | Isolate old/Add new parameters for training. For example LORA method                         |
| Soft prompting                             | Few, new parameters | Labeled, task-specific | Learnable prompt params   | Adding params to prompt                                                                      |
| Continual Pre-Training                     | All parameters      | Unlabeled              | Same as LLM pre-training  | Training the model to predict the next word from millions of words of the specialized domain |

## Inference
- Process of using the custom model to predict


![[LLM Training Hardware Costs.png]]

> Cramming: Training a Language Model on a Single GPU in One Day:
> https://arxiv.org/pdf/2212.14034





## GPU and Inferencing
- GPU memory is limited, hence switching between midels can incur significant overhead due to reloading the full GPU memory.
- Custom models derived from the same base model can be used in the same GPU cluster as these models share the majority of weights, with only slight variations. --> Results in minimal overhead when switching between models.



## Techniques:

#### Vanilla Fine Tuning:
- Involves updating the weights of all the layers in the model.
- Requires longer training time and higher serving (inference) costs.
#### T-Few Fine Tuning
- Selectively updates only a fraction of the model's weights.
- Process:
	- Start with the base model weights and annoted training data (labeled dataset).
	- Generate T-Few Fine-Tuning Method
	- Feed this to few layers, and then Fine Tune.



## Fine-Tuning Parameters:
1. Total Training Epochs
2. Batch Size
3. Learning Rate
4. Early stopping threshold
5. Early stopping patience
6. Log model metrics interval in steps



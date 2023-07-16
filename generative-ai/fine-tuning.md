#### Fine tuning
- Supervised learning process where you use a data set of labeled examples to update the weights of the LLM
- Helps to generate completions for specific task
- Instruction fine tuning
  - Improves model's performance on a variety of tasks
  - If all model weights are updated, it is called full fine tuning
- Results in a new model called instruct model

#### Fine tuning on single task
- Fine-tune model to improve performance on single task
- Catastrophic forgetting
  - options to avoid
    - fine-tuning on multiple tasks at one time
    - Perform parameter efficient fine-tuning or PEFT

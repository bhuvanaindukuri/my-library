#### OM
#### LLM - Large Language Models
- Prompts - Text passed to LLM window
- Context window - Space or memory that is available to the prompt
- Completion - Output of the model
- Inference - Act of using the model to generate text
- Prompt Engineering - Improving the prompt for better outcome

  
#### Tranformer Architecture
- Paper by Google & University
- 2 components
  - Encoder
  - Decoder
- Stages
  - Tokenizer
    - Convert words to numbers
    - Could be the position of the word in the dictionary
    - Should use the same one for train and generate
  -  Embedding
    - Represents numbers as vectors
    - Vectors store context of the word as well
    - Size of the vector in paper was 512
  - Positional encoding
    -  Saves positions of the words
  -  Multi-headed self attention
    - Finds the relation of each word with another word
    - Number of attention heads could vary by model between 12-100 
    - Each self-attention head will learn a different aspect of language.
  - Feed forward network
    - The output of this layer is a vector of logits proportional to the probability score for each and every token in the tokenizer dictionary.
  - Softmax layer
    - The logits are normalized into a probability score for each word
- Types of Transformer Models
  - Encoder Only Models
    - Not frequently used
    - Can be used for sentiment analysis with architecture changes
  - Encoder Decoder Models
    - Perform well on sequence-to-sequence
    - Good for translation kind of tasks  
    - Examples: BART , T5
  - Decoder only models
    - Most widely used
    - Examples: GPT family of models, BLOOM, Jurassic, LLaMA, and many more

#### In-context Learning
- Zero-Shot Inference
  - Provide instructions and format
  - No example
- One shot inference
  - Provide single example in the prompt
  - Examples can help smaller models better
- Few shot inference
  - Multiple examples

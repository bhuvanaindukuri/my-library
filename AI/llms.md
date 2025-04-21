### Definitions
- Dimensions - Number of values in an vector
- Attention
  - Allows a model to focus on parts of input that are relevant to one another. Helps while generating embeddings for large complex sentences.
  - Generally used in encoders and decoders in RNNs
  - Avoid leakage of context
- Transformer
  - Has encoder and decoder
  - Works well for translation
- Context Length
  - Maximum number of tokens a generative LLM can process
  - Includes generated tokens
### Tokenization
- Used to split sentence to embeddings
- Has defined vocabulary
- Sometimes splits the words if the word doesnt exist in vocabulary
- \## is used to indicate that the token is a continuition of the previous one. In bert model
- Larger the vocabulary lesser the number the tokens but higher the number of embeddings to be processed
- bert-base-uncased model has vocab length of 30K while Xenova/gpt-4 has around 100K
- Other encoder models : gpt2, google/flan-t5-small, bigcode/starcoder2-15b, microsoft/Phi-3-mini-4k-instruct, Qwen/Qwen2-VL-7B-Instruct

### Transformer LLM
- Consists of
  1) Tokenizer
  2) Series of transformer blocks
      1) Self Attention
         1) Relevance scoring
         2) Combining information
      2) Feed Forward Neural Network      
  3) LM Head 

### Attention
- Split into multiple attention heads
- Has key & value metrices
- Types of attention
  - Full attention
    - Considers all the previous tokens
  - Sparse transformer (Strided)
    -  Considers last X tokens always
  - Sparse transformer (Fixed)
    - No of tokens varies from 0 to X
  - Ring attention
 
### Mixture of Expert MOE
- Applicable in Feed Forward Neural network(FFNN)
- Components
  - Router
  - Experts  
- Each layer is split into multiple experts
- one expert is chosen in each layer
- Router identifies the right expert.
  - Router is a small NN itself.
  - Generates probability scores for each expert based on input
- Examples of experts: Punctuation, verbs, conjunctions
- In a sparse model only a subset of experts is activated at a given time 

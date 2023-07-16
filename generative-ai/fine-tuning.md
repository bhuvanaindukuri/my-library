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

#### FLAN ( Fine-tuned language net )
- Instruction model
- FLAN models refer to a specific set of instructions used to perform instruction fine-tuning
- Metaphorical dessert to the main course of pretraining
- Examples
  - FLAN-T5
  - FLAN-PALM
    - SAMsum

#### Evaluation Metrics
- ROUGE
  - Recall Oriented Understudy for Gisted Evaluation
  - Used for Text Summarization
  - Metrics ROUGE-1
    - Recall = Unigram matches / unigrams in reference
    - Precision = Unigram matches / Unigrams in output
    - F1 = 2* (Precision * Recall ) / (Precision + Recall)  
  - Metrics ROUGE-2
    - Recall = Bigram matches / Bigrams in reference
    - Precision = Bigram matches / Bigrams in output
    - F1 = 2* (Precision * Recall ) / (Precision + Recall)  
  - Metrics ROUGE-L
    - Recall = LCS (Gen, Ref) / Unigrams in reference
    - Precision = LCS (Gen, Ref) / Unigrams in output
    - F1 = 2* (Precision * Recall ) / (Precision + Recall)      
- BLEU SCORE
  - Bi-lingual Evalution Understudy
  - Metrics
    - Avg ( Precision across range of n-gram sizes )
- Terminology
  - Unigram - Single Word
  - Bigram - Combination of 2 words 
  - LCS - Longest Common Subsequence
  - Clip - Function to deduplicate the matches
 
 #### Evaluation Benchmarks
 - GLUE ( General Language Understanding Evaluation )
 - SuperGLUE
 - HELM ( Holistic Evaluation of Language Models )
   - Accuracy
   - Calibration
   - Robustness
   - Fairness
   - Bias
   - Toxicity
   - Efficiency
 - MMLU (Massive Multitask Language Understanding)
 - Big-bench

#### PEFT
- Trade-offs
  - Parameter Efficiency
  - Memory Efficiency
  - Training Speed
  - Model Performance
  - Inference Costs
- Methods
  - Selective
  - Reparametirization Ex: LoRA
    - Low Rank Adaptation ( LoRA)
      - Build matrices for each task and replace when required
  - Additive
    - Adapters
    - Soft Prompts
      - Prompt Tuning


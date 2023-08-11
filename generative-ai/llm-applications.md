#### Challenges in LLMs
- Out of Date / Knowledge cutoff
  - Connect to external data sources and APIs to mitigate Ex: LangChain
  - Retrieval Augmented Generation (RAG)  - 
    -  Framework for building LLM powered systems that make use of external data sources
- Wrong/ Lack of reasoning
  - Chain of thought prompting
    - Adding chain of thought to prompt text might help
  - Program-aided Language(PAL) models
    - LLM + Code Interpreter
    - Models that offload computational tasks to other programs.
- 

#### ReAct - Reasoning and Action
- Prompting strategy that combines chain of thought reasoning with action planning
- Uses structured examples to show a large language model how to reason through a problem and decide on actions to take that move it closer to a solution
- Solve question answering task with interleaving Thought, Action and Observation steps.
- Action can be 3 types
  - Search
  - Lookup
  - Finish

#### LLM Application Architecture
-  Infrastructure
-  Data
  - Information Sources
  - LLM Models
  - Generated Outputs & Feedback
- LLM Tools & Frameworks - LangChain, Model Hubs
- Application Interfaces

#### Key terms
- Proximal Policy Optimization (PPO)
  - The constraint that limits the distance between the new and old policy
- KL Divergence
  - KL divergence is used to enforce a constraint that limits the extent of LLM weight updates.
  - KL divergence measures the difference between two probability distributions.
- LangChain
  - The LangChain framework is built around LLMs and allows the chaining of various components to create more advanced applications for LLMs. It supports use cases like chatbots, Generative Question-Answering (GQA), and summarization.

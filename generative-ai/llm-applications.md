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

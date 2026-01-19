# Formal AI Agents for Model Checking Concurrent Programs

- LangChain (https://www.langchain.com) AI agent implementations calling a local model checker to temporal model check concurrent implementations expressed with a finite state machine description.
- The agents call a local model checker binary and then summaries the result of the model checking.
- I used
  - NuSMV (https://nusmv.fbk.eu) as a symbolic model checker which is based on Binary Decision Diagrams (BDDs).
  - OpenRouter (https://openrouter.ai) as a free API provider.
  - A Mistral AI (https://mistral.ai) LLM as the reasoning model.
  - ChatGPT (https://chatgpt.com/) for the most of the functionalities of the implementation which includes guardrails.
- The user only needs to provide the name of the program (.smv) or a directory that is to be model checked.
- The implementations are
    - FormalAgent.ipynb is designed for a single program.
    - FormalAgentDir.ipynb is designed for all programs in a directory.
    - MultiFormalAgents.ipynb is designed for multi-agents working together for all programs in a directory. However, *the interpretation of the mutex.smv becomes incorrect as compared to the correct interpretation of a single agent*.
    - MultiFormalAgentsWithReflection.ipynb is designed for multi-agents with reflection working together for all programs in a directory. *The interpretation of the mutex.smv is still incorrect. Reflection does not correct the incorrect interpretation*. 


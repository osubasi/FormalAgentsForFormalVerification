# Formal Agents for Model Checking Concurrent Programs

- Two LangChain (https://www.langchain.com) AI agent implementations calling a local model checker to temporal model check concurrent implementations expressed with a finite state machine description.
    - FormalAgent.ipynb is designed for a single program.
    - FormalAgentDir.ipynb is designed for all programs in a directory.
- The agents call a local model checker binary and then summaries the result of the model checking.
- I used
  - NuSMV (https://nusmv.fbk.eu) as a symbolic model checker which is based on Binary Decision Diagrams (BDDs).
  - OpenRouter (https://openrouter.ai) as a free API provider.
  - A Mistral AI (https://mistral.ai) LLM as the reasoning model.
  - ChatGPT (https://chatgpt.com/) for the most of the implementation which includes guardrails.
- The user only needs to provide the name of the program (.smv) or a directory that is to be model checked.


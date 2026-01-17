# Formal Agent for Model Checking Software

- A LangChain (https://www.langchain.com) AI agent implementation calling a local model checker to temporal model check concurrent implementations expressed as a finite state machine description.
- The agent calls a local model checker binary and then summaries the result of the model checking.
- I used NuSMV ((https://nusmv.fbk.eu)) as a symbolic model checker which is based on Binary Decision Diagrams (BDDs).
- I used OpenRouter (https://openrouter.ai) as a free API provider.
- I used a Mistral AI (https://mistral.ai) LLM as the reasoning model.
- I used ChatGPT (https://chatgpt.com/) for the most of the implementation.

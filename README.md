# LangGraph-simple-project
The idea of that project is to find gaps in the flow of a request in a distributed system. The flow is described in natural language and the gaps are found by an LLM.

Input: A description of the flow of a request in a distributed system, written in natural language.
Output: State, where the flow is the final one

There is human in the loop always! If the implementation which covers all of the criteria of each agent is not found after X amount of iterations a human MUST decide what will be the flow by writing it manually.
If the implementation is found, the human MUST approve it or ask for a new one.

Responsibility is in the always in the Human, so we want verification even if all agents agreed that the flow is good enough.

This is a simple project to demonstrate the usage of langraph. There are no real external systems like Databases, some fancy services, etc.

It uses
- Web search
- Youtube search tool
- LLM (OpenAI)

Code quality is not the one you expect to see - a lot of hardcoded values, etc.

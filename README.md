# LangGraph-simple-project
The idea of this project is to find gaps in the flow of a request in a distributed system. The flow is described in natural language and the gaps are found by an LLM.

Input: A description of the flow of a request in a distributed system, written in natural language.
Output: State where the flow is the final one

There is always a human in the loop! If an implementation that covers all of the criteria of each agent is not found after X iterations, a human MUST decide the flow by writing it manually.
If an implementation is found, the human MUST approve it or ask for a new one.

Responsibility is always with the human, so we want verification even if all agents agree that the flow is good enough.

This is a simple project to demonstrate the usage of langraph. There are no real external systems like databases or other fancy services.

It uses
- Web search
- YouTube search tool
- LLM (OpenAI)

Important notes:

- Code quality is not what you expect to see - a lot of hardcoded values, etc.
- Flows, proposals from humans, and agents' system prompts are all super short for the sake of readability and demonstration. In real life they should be much more detailed and precise!
- No special attention was paid to exception handling. In a real project that should be much more precise and cover all possible edge cases.
- Unfortunately, the flow where all agents agree on a solution is not demonstrated, as it never happens in these examples, so more formal criteria should be added to be able to have more definitive results.
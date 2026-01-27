**Conversational Knowledge Bot**

# Overview:
This project implements a Conversational Knowledge Bot using LangChain,
Groq LLM, Wikipedia tools, and conversation memory. The bot can answer
factual questions, remember previous conversation context, and interact
through a command-line interface (CLI). This project fulfills Task 2:
Conversational Knowledge Bot from the Soulpage GenAI assignment.

# Features:
Conversational chat interface (CLI-based) - Context-aware responses
using conversation memory - External knowledge retrieval via Wikipedia -
Groq-hosted LLM (\`llama-3.1-8b-instant\`) - User-friendly "Please
wait..." message during response generation - Clean console output with
suppressed deprecation warnings

# Example Usage:
Groq LLM initialized 
Memory initialized 
Wikipedia tool ready 
Agent initialized successfully

Conversational Knowledge Bot Type 'exit' or 'quit' to stop

You: Who is the CEO of Microsoft? Bot: Satya Nadella is the CEO of
Microsoft.

You: Where did he study? Bot: He studied at Manipal Institute of
Technology and the University of Chicago.

# Architecture & Flow
User Input
↓
AgentExecutor
↓
ConversationalChatAgent
↓
┌───────────────┐
│ Conversation │ (ConversationBufferMemory)
│ Memory │
└───────────────┘
↓
Wikipedia Tool (External Knowledge)
↓
Groq LLM (Response Generation)
↓
Bot Output


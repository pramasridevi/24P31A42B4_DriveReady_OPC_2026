# Day 3 – Advanced AI Shopping Assistant using LangChain

## Overview
Day 3 focuses on improving the Kiran Shop AI assistant using advanced LangChain components, prompt templates, conversation history and automated response testing.

The implementation introduces structured prompt management, output parsing, CSV-based test cases and LangChain agent creation.

## Objectives
- Understand LangChain prompt templates.
- Work with conversation history using `MessagesPlaceholder`.
- Build reusable LLM chains.
- Implement multi-turn conversations.
- Evaluate chatbot responses using CSV test cases.
- Explore LangChain agent creation.

## Technologies Used
- Python
- LangChain
- LangChain-Groq
- Groq API
- CSV
- Google Colab

## Implementation

### 1. LLM Configuration
- Integrated Groq LLM using `ChatGroq`.
- Configured the `openai/gpt-oss-120b` model.
- Set the temperature to 0.1 for response generation.

### 2. Prompt Template Creation
Used LangChain components:
- `ChatPromptTemplate`
- `MessagesPlaceholder`
- `StrOutputParser`

Created a structured system prompt defining the shopping assistant's role, responsibilities and response guidelines.

### 3. Chain Creation
Built an LLM processing chain using:

`prompt | llm | StrOutputParser()`

This chain processes customer questions and generates text responses.

### 4. Conversation History
Implemented an `ask()` function to maintain conversation history.

The assistant stores previous human and AI messages, allowing it to respond with conversational context.

### 5. CSV-Based Testing
Created a `run_tests()` function to evaluate chatbot responses using test cases stored in a CSV file.

The testing process:
- Reads questions from a CSV file.
- Sends each question to the AI chain.
- Checks whether the expected text is present in the response.
- Displays PASS or FAIL for each test.
- Calculates the overall test pass percentage.

### 6. LangChain Agent Creation
Explored LangChain's `create_agent()` functionality.

Created an agent using the configured LLM and system prompt. The implementation currently uses an empty tools list.

## Key Learnings
- Advanced LangChain prompt management.
- Building LLM chains.
- Using output parsers.
- Managing conversational context.
- Testing AI-generated responses.
- Reading and processing CSV files.
- Introduction to LangChain agents.

## Project Outcome
Developed an enhanced AI shopping assistant with structured prompts, conversational history, automated response testing and an introduction to agent creation.

## How to Run
1. Open the Day-3 notebook in Google Colab.
2. Install the required LangChain dependencies.
3. Configure the Groq API key in Colab Secrets.
4. Make sure the test CSV file is available at the configured path.
5. Execute the notebook cells sequentially.

---
**Workshop:** 12 Days of Agentic AI  
**Day:** 03
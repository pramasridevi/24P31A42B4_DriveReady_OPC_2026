# Day 2 – Building an AI Shopping Assistant with Memory

## Overview
Day 2 focuses on managing product information, calculating prices and developing a conversational AI shopping assistant for **Kiran Shop**.

The implementation combines Python dictionaries, JSON handling, functions and LangChain-Groq to create an interactive shopping experience.

## Objectives
- Store and manage product information using Python dictionaries.
- Retrieve product prices and calculate total costs.
- Understand JSON serialization and deserialization.
- Handle unavailable products.
- Integrate Groq LLM with LangChain.
- Implement conversational history for multi-turn interactions.

## Technologies Used
- Python
- LangChain
- LangChain-Groq
- Groq API
- JSON
- Google Colab

## Implementation

### 1. Product Menu Management
Created a Python dictionary containing grocery products and their prices.

| Product | Price (₹) |
|---|---:|
| Rice | 60 |
| Sugar | 45 |
| Wheat Flour | 50 |
| Tea Powder | 75 |
| Coffee Powder | 120 |
| Milk | 30 |
| Curd | 40 |
| Soap | 45 |
| Shampoo | 80 |
| Toothpaste | 55 |
| Biscuits | 20 |
| Chips | 20 |
| Cooking Oil | 150 |
| Salt | 25 |
| Detergent | 90 |

### 2. Dictionary Operations
- Accessed product prices using dictionary keys.
- Used `get()` to handle missing product names.
- Explored dictionary key lookup and error handling.

### 3. JSON Operations
- Converted Python dictionaries into JSON strings using `json.dumps()`.
- Converted JSON strings back into Python objects using `json.loads()`.

### 4. Price Calculation
Implemented the `get_price()` function to calculate the total cost based on product price and quantity.

### 5. AI Shopping Assistant
- Configured Groq LLM using LangChain.
- Designed a system prompt with shop details and product prices.
- Created an `ask()` function to answer customer questions.

### 6. Conversational Memory
Implemented conversation history using a message list.

The chatbot maintains previous user and assistant messages, allowing it to handle multi-turn conversations.

An exit condition is provided using `bye`, `exit` or `quit`.

## Key Learnings
- Python dictionaries and data management.
- JSON serialization and deserialization.
- Functions and exception handling.
- Product price calculation.
- LLM integration using LangChain.
- Maintaining conversational history.
- Building interactive AI applications.

## Project Outcome
Developed an interactive AI shopping assistant with product information, price calculation and conversational memory.

## How to Run
1. Open the Day-2 notebook in Google Colab.
2. Install the required dependencies.
3. Configure the Groq API key in Colab Secrets.
4. Execute the notebook cells sequentially.
5. Interact with the chatbot using grocery-related questions.

---
**Workshop:** 12 Days of Agentic AI  
**Day:** 02
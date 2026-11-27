# Day 4 – AI-Powered Home Bakery Order Assistant 🍰

## 📌 Overview

Developed an AI-powered Home Bakery Order Assistant using **LangChain and Groq LLM** that interacts with customers through natural language conversations.

The assistant helps customers check bakery opening hours, calculate cake prices, and place orders. It uses custom tools to retrieve information and stores confirmed orders directly in Google Sheets.

This project demonstrates how AI agents can use tools to perform real-world tasks instead of simply generating text responses.

## ✨ Features

- **AI-Powered Conversations:** Understands and responds to customer queries naturally.
- **Price Calculation:** Provides accurate cake prices based on menu items and quantities.
- **Opening Hours Checker:** Checks bakery operating hours for any day of the week.
- **Order Management:** Collects customer details, cake selection, quantity, pickup date, and eggless preference.
- **Eggless Cake Options:** Supports customer preferences for eggless cakes.
- **Google Sheets Integration:** Automatically saves confirmed orders in Google Sheets.
- **Conversation Memory:** Maintains chat history to support continuous conversations.
- **Order Confirmation:** Provides order details and the calculated total after successful saving.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| LangChain | AI agent creation and orchestration |
| LangChain Groq | LLM integration |
| Groq LLM | Natural language understanding |
| Pydantic | Order data validation |
| Google Colab | Development and execution environment |
| gspread | Google Sheets integration |
| Google Authentication | Secure Google account access |

## 🤖 AI Agent Tools

The agent uses three custom tools:

### 1. `get_price()`
- Retrieves the price of a selected cake.
- Calculates the total based on quantity.
- Checks whether the requested item exists in the menu.

### 2. `is_open()`
- Checks bakery opening hours.
- Accepts the day of the week.
- Returns the corresponding operating hours.

### 3. `log_order()`
- Validates customer order information using Pydantic.
- Calculates the total order amount.
- Saves confirmed order details to Google Sheets.

## 🍰 Bakery Menu

| Cake Item | Price (₹) |
|---|---:|
| Plum Cake | 500 |
| Chocolate Cake | 650 |
| Cupcake | 80 |

**Opening Hours:**
- Monday – Saturday: 9 AM – 8 PM
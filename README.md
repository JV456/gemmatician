# Gemmatician - MathsGPT

Welcome to my **Gemmatician - MathsGPT** – an end-to-end generative AI application powered by Google Gamma! This app is built using Streamlit and leverages the latest AI models and agent toolchains to provide dynamic step-by-step solutions for math and logical reasoning problems.

---

## ✨ Features

- **Chatbot Interface:** Ask math questions in natural language and get step-by-step explanations.
- **Supports Logical Reasoning:** Not just calculations–get thoughtful answers to logical and multi-step problems.
- **Integrated Wikipedia Search:** Fetches relevant information for queries requiring background knowledge.
- **Persistent Chat History:** Conversations are maintained for session continuity using Streamlit's session state.
- **Agent-Based Toolchain:** Combines multiple tools (calculator, Wikipedia, logic/reasoning) with Google Gamma's LLM for robust results.

---

## 🛠️ How It Works

### Architecture

- **Streamlit** provides the frontend and stateful chat interface.
- **Google Gamma (via Grok API):** The backbone LLM for all generative and reasoning tasks.
- **Tools & Agents (Langchain):**
  - **Wikipedia Tool:** Handles search and fetch queries.
  - **Calculator Tool:** Parses and solves mathematical expressions.
  - **Reasoning Tool:** Runs custom prompts with the LLM to solve multi-step or logic-based queries.

### Flow

1. **User inputs a math or logic question.**
2. **Agent orchestrates** the required tools based on the task:
    - For direct math: Calculator Tool
    - For context/knowledge: Wikipedia Tool
    - For logic/reasoning: Reasoning Tool (LLM chain with a prompt template)
3. **Step-by-step response**, often with pointwise explanations, is displayed in the chat interface.
4. **Session history** is maintained, and every new question/answer is appended to the chat.

---

## 📝 Example Usage and Output


<img width="1919" height="867" alt="Screenshot 2025-07-19 205811" src="https://github.com/user-attachments/assets/c9f7f814-6b9e-4ba0-9daa-a0bee247d71c" />

<img width="1919" height="871" alt="Screenshot 2025-07-19 205820" src="https://github.com/user-attachments/assets/dacc7acc-e244-40c5-b0a5-5cdf662d6f3e" />

---

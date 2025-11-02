# Utility Billing Multi-Agent Conversational Chatbot

This project implements a **multi-agent conversational AI system** to support customer billing inquiries in the utility services domain (such as gas, water, or electricity companies). The goal is to provide accurate, context-aware, and human-like responses by decomposing the chatbot into multiple specialized agents controlled by a central **Manager Agent**.

---

## Objective

To automate customer support for billing queries by enabling the chatbot to:
- Understand user intent
- Retrieve and extract bill details from PDF bills
- Explain bill components in simple language
- Escalate unresolved or complaint-related queries
- Collect customer feedback to improve service

---

## System Architecture

The system is composed of **six specialized agents**, each responsible for a specific part of the conversation:

1. **Manager Agent**
   - Orchestrates tasks and decides which agent should take action next based on context.

2. **Intent Recognition Agent**
   - Identifies what the customer is asking (e.g., bill amount inquiry, due date query, complaint).

3. **Bill Extraction Agent**
   - Parses and extracts structured data from PDF bills (meter usage, bill amount, taxes, due date, etc.).

4. **Billing Explanation Agent**
   - Converts bill data into simple explanations that customers can easily understand.

5. **Escalation Agent**
   - Handles scenarios where the user is dissatisfied or when issues require human support.

6. **Feedback Agent**
   - Collects customer experience feedback at the end of the interaction.

---

## Conversation Flow

- User Message → Intent Recognition Agent
- Manager Agent (decision point)
- Bill Extraction Agent (if needed)
- Billing Explanation Agent
- Escalation Agent (if required)
- Feedback Agent (conversation closure)


---

## Features

- Natural language understanding of billing questions
- Automated PDF bill reading and structured data extraction
- Friendly, human-readable billing breakdown
- Complaint escalation logic
- End-of-chat feedback collection

---

## Tech Stack

- **Python**
- **LLM / Chat Model:** OpenAI / HuggingFace
- **PDF Parsing:** PyMuPDF
- **Agent Orchestration:**  Manager agent routing logic
- **UI (optional):** Streamlit

---

## Installation

```bash
git clone https://github.com/<your-username>/utility-billing-multi-agent-chatbot.git
cd utility-billing-multi-agent-chatbot
pip install -r requirements.txt
streamlit run app.py


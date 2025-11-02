# CallSenseAI
A Multi-Agent AI System for Banking Call Transcript Behavioural Analysis

CallSenseAI is a multi-agent conversational analytics system designed to automatically analyze customer service call transcripts in banking environments. The system identifies **customer intent**, **sentiment**, and **root cause issues** to support Quality Assurance teams and improve customer satisfaction.

---

## 🔍 Project Overview

Banks handle thousands of customer support calls daily. Manual review is slow, inconsistent, and expensive. CallSenseAI automates this process using a multi-agent architecture that collaborates to analyze transcripts and produce actionable insights.

The system is accessed via a chatbot interface, allowing QA teams to upload transcripts and receive structured feedback instantly.

---

## 🧠 System Architecture

The system consists of **four AI Agents**:

| Agent | Purpose |
|------|---------|
| **Supervisor Agent** | Manages workflow, delegates tasks, aggregates final outputs |
| **Intent Classification Agent** | Classifies customer goal from 14 predefined banking intents (e.g., balance inquiry, loan request, card issue) |
| **Sentiment Analysis Agent** | Evaluates emotional tone at multiple points in the conversation |
| **Root Cause Analysis Agent** | Determines underlying issue, friction points, and preventable problems |

Agents communicate through prompt-based or LLM-based coordination.

---

## 🏦 Sample Supported Banking Intents

- Account balance enquiry  
- Credit/Debit card blocked  
- Loan enquiry or application  
- Transaction dispute  
- Online banking login issue  
- Account upgrade  
- Fraud or suspicious activity report  
*(Total: 14 predefined intents)*

---

## 🧾 Key Features

- ✅ Multi-Agent Reasoning Architecture  
- ✅ Works with any call transcript (text form)  
- ✅ Identifies emotional sentiment trends  
- ✅ Detects core customer frustration drivers  
- ✅ Provides summary & improvement recommendations  
- ✅ Chatbot interface for QA teams  
- ✅ Modular and scalable design

---

## 🏗️ Tech Stack

| Component | Technology |
|---------|------------|
| Language Model | GPT-4 / GPT-5 / LLaMA 3 or similar |
| Framework (optional) | LangChain / CrewAI / Haystack |
| Backend | Python |
| Interface | Streamlit / Gradio / Chat UI |
| Storage | Local / Cloud / Vector DB (optional) |

---

## 🚀 How to Run

```bash
# Clone the repository
git clone https://github.com/your-username/CallSenseAI.git
cd CallSenseAI

# Install dependencies
pip install -r requirements.txt

# Run the chatbot app
python app.py

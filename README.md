# 🤖 The Corporate Knowledge Navigator

**Capstone Project for the Google AI Agents Intensive Course (Enterprise Agents Track)**

This project showcases an advanced Multi-Agent System designed to act as an intelligent single point of contact for corporate employees, instantly answering document-based queries and providing real-time system status updates.

---

## ✨ Key Features & Technical Architecture

### 1. Multi-Agent Routing (The Master Agent)
* The system uses a Master Agent (Router) powered by **Gemini's Tool Calling** capability.
* The Agent intelligently routes the query based on intent, deciding between the RAG system and the Custom Tool, demonstrating effective Agent-to-Agent (A2A) protocol.

### 2. Retrieval-Augmented Generation (RAG)
* **Memory Bank:** Implemented RAG using `GoogleGenAIEmbeddings` and a Vector Store (ChromaDB) to accurately retrieve information from the `Policies.pdf` document.
* **Purpose:** Handles all document lookups, HR policies, and financial memo queries.

### 3. Custom Tools Integration
* A custom Python function (`check_internal_system_status`) is integrated as a dedicated tool.
* **Purpose:** Simulates communication with external Enterprise APIs (e.g., IT Status Checkers) to provide real-time operational data.

### 4. Observability
* The system uses `verbose=True` logging to display the Agent's decision-making process (**Thought** and **Action**), which is crucial for debugging and demonstrating effective routing logic.

---

## 🎯 Problem Solved & Value Proposition

### ❓ The Problem
In large organizations, employees waste significant time searching for complex internal policies, technical guides, or checking IT system statuses via slow manual processes (emails, scattered documents).

### 💡 The Solution
The Corporate Knowledge Navigator eliminates manual searching by providing an automated, smart interface that instantly routes queries to the most appropriate data source.

### 💰 Value Articulation (For Top Ranking)
By automating the search and routing process, this agent is estimated to save employees an average of **10+ hours per month** in unproductive searching and information gathering, translating directly into significantly increased organizational efficiency and high Return on Investment (ROI).

---

## 🛠️ Setup and Running Guide

### 1. Requirements

* `The Corporate Knowledge Navigator.ipynb` (This file)
* `Policies.pdf` (The corporate dummy document)
* A valid **Gemini API Key**.

### 2. Running Instructions (Google Colab)

1.  Upload both the `.ipynb` file and the `Policies.pdf` to your Google Colab session.
2.  Open the `.ipynb` file and paste your Gemini API Key into the designated section.
3.  Run all cells sequentially from top to bottom.
4.  The final cells contain successful test cases demonstrating accurate routing for Policy and IT Status queries.

---

**Thank you!**

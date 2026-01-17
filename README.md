# 🧠 Building a Multi-Agent AI with LangChain & LangGraph

## 📌 Overview

This project demonstrates how to build a **multi-agent AI system** using **LangChain** and **LangGraph**, where multiple specialized agents collaborate to generate code, write documentation, and create unit tests based on a given software task.

The system showcases **agent orchestration**, **state management**, and **workflow control** using graph-based execution.

---

## 🚀 Key Features

* Multi-agent architecture using **LangGraph**
* Specialized agents for:

  * Code generation
  * Documentation writing
  * Unit test creation
* Graph-based workflow execution
* Modular, scalable, and reusable design
* Interactive CLI for agent selection

---

## 🧩 Architecture

The system uses a **shared state** that flows between agents:

```text
User Input → Code Generator → Documentation Writer → Test Writer
```

Each agent operates independently while sharing context through a common state object.

---

## 🛠️ Tech Stack

* **Python**
* **LangChain**
* **LangGraph**
* **OpenAI (ChatOpenAI)**
* **TypedDict for state management**

---

## ⚙️ Agents Description

### 1️⃣ Code Generator Agent

* Converts a natural language task into clean, executable Python code.

### 2️⃣ Documentation Writer Agent

* Generates concise documentation explaining the generated code.

### 3️⃣ Test Writer Agent

* Creates unit tests to validate the generated code.

### 4️⃣ Full Pipeline

* Executes all agents sequentially using LangGraph edges.

---

## ▶️ How to Run

### 1. Install Dependencies

```bash
pip install langchain langgraph langchain-openai
```

### 2. Set API Key

```bash
export OPENAI_API_KEY="your-api-key"
```

*(Windows PowerShell: `setx OPENAI_API_KEY "your-api-key"`)*

---

### 3. Run the Application

```bash
python main.py
```

---

### 4. Example Interaction

```text
Enter software task: Create a Python program to check if a number is prime

Choose an agent:
1. Code Generator
2. Documentation Writer
3. Test Writer
4. Full Pipeline

Select option (1-4): 4
```

---

## 📂 Project Structure

```text
multi-agent-ai-langgraph/
│── main.py
│── agents/
│   ├── code_generator.py
│   ├── documentation_writer.py
│   ├── test_writer.py
│── README.md
```

---

## 🧠 Learning Outcomes

* Understand **agent-based AI systems**
* Learn **graph-driven orchestration** using LangGraph
* Implement **stateful multi-agent workflows**
* Build scalable AI pipelines using LangChain

---

## 📈 Use Cases

* Automated code generation pipelines
* AI-assisted software development
* Intelligent documentation and testing systems
* Research and experimentation with agentic AI

---

## 🔮 Future Enhancements

* Add parallel agent execution
* Integrate memory and tool usage
* Support multiple programming languages
* Add evaluation and feedback loops

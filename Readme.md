# DataWizard: AI-Powered Data Analysis Agent

## Overview

DataWizard is an AI-powered data analysis assistant built using LangChain and OpenAI models. It enables users to interact with datasets using natural language and automates core data science workflows such as dataset discovery, summarization, and machine learning evaluation.

The system is designed to reduce manual effort in exploratory data analysis and make advanced analytics accessible through conversation.

---

## Objectives

1. Build custom LangChain tools for data workflows  
2. Implement an in-memory dataset caching system  
3. Create a natural language interface for analytics  
4. Develop a multi-step reasoning agent  
5. Automate classification and regression evaluation  
6. Enable conversational data science  

---

## Key Features

1. Dataset Discovery  
Automatically detects available CSV files in the working directory.

2. Dataset Caching  
Stores datasets in memory to avoid repeated loading and improve performance.

3. Dataset Summarization  
Provides schema-level insights including column names and data types.

4. Dynamic DataFrame Execution  
Supports execution of Pandas methods such as:
- head  
- tail  
- describe  
- info  

5. Machine Learning Evaluation  
Includes:
- Classification using Random Forest with accuracy  
- Regression using Random Forest with R² and Mean Squared Error  

6. Autonomous AI Agent  
Uses a ReAct-based architecture to:
- Reason step by step  
- Select tools dynamically  
- Execute workflows  

7. Natural Language Interface  
Allows users to query datasets without writing code.

---

## Architecture

1. Tools Layer  
Custom LangChain tools for:
- File discovery  
- Data loading and caching  
- Data summarization  
- DataFrame operations  
- Model evaluation  

2. Agent Layer  
Handles reasoning and tool selection using LangChain agent framework.

3. Execution Layer  
Managed by AgentExecutor to perform multi-step reasoning loops.

4. LLM Layer  
OpenAI model integrated via LangChain.

---

## Tech Stack

- Python 3.8+
- LangChain
- OpenAI
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

---

## Installation and Setup

```bash
git clone https://github.com/your-username/datawizard.git
cd datawizard

pip install langchain-openai==0.3.10
pip install langchain==0.3.21
pip install openai==1.68.2
pip install pandas==2.2.3
pip install numpy==2.2.4
pip install matplotlib==3.10.1
pip install seaborn==0.13.2
pip install scikit-learn==1.6.1

export OPENAI_API_KEY="your_api_key_here"

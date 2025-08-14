# AI Agent to Retrieve Data from MongoDB

This project implements an AI-powered query agent that generates, executes, and interprets result using **LangGraph**, **MongoDB** and **Docker**. It is designed to answer natural language questions about a MongoDB database, process results, and provide concise answer.

---

## Features

•	Automatically generates MongoDB pipelines from plain English questions.  
•	Executes queries on MongoDB and retrieves results.  
•	Formats query results into concise, human-readable answers.  
•	Fully modular and extensible with LangGraph.

---

## Project Structure

├── agent_with_mongodb.ipynb        # AI agent logic and architecture  
├── insert_data_mongo.py            # Data entry in MongoDB  
├── docker-compose-infra.yml        # Docker setup for MongoDB  
├── README.md                       # Project documentation

---

## How It Works
1. State-based Agent:
   - generate_pipeline: Generates MongoDB aggregation pipeline from natural language.
   - execute_query: Executes the pipeline against MongoDB and fetches results.
   - format_answer: Formats the results into a concise, human-readable answer.

2. Pipeline Parsing:
   - Handles nested dictionaries and lists in aggregation pipelines.

3. LLM Integration:
   - Uses language model by Groq LLaMA3-70B and LangGraph.
   - Generate valid MongoDB pipelines.
   - Format query results into readable answers.

---

## Process

1. Configure Docker.
2. Configure MongoDB.
3. Insert data in MongoDB database.
4. Run agent code to retrieve data from database.

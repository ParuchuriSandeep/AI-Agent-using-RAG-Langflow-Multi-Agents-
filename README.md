Project: Multi-Agent AI Customer Support System

Problem Statement:
We addressed the challenge of providing efficient and comprehensive customer support, particularly when dealing with complex data like order information and product details. Traditional methods often involve manual lookups and fragmented information,leading to slow response times and inconsistent answers.We built an intelligent customer support system that seamlessly accesses and synthesizes data from multiple sources, providing accurate and timely responses to customer inquiries.

Project Abstract:

This project successfully developed a multi-agent AI application using Langflow. The system handles customer support tasks by integrating Retrieval Augmented Generation (RAG) with database queries. It comprises several specialized agents, including an order lookup agent, a product information retriever, and an FAQ responder, all managed by a central orchestrator. We leveraged Astra DB, a vector database, to efficiently store and retrieve relevant information. A user-friendly interface was created using Streamlit to enable seamless interaction with the AI system. The complete project codebase has been pushed to Git.

Project Summary:

The following key steps were undertaken:

Foundation – 

Basic AI Agent Setup (Langflow):

A foundational Langflow flow was created.
"Chat Input," an LLM node (e.g., OpenAI's GPT), and "Chat Output" nodes were implemented.
The LLM node was configured with API keys.
Basic chat functionality was tested and verified.Data Integration – Vector Database 

(Astra DB):

Astra DB was integrated for data retrieval.
An "Astra DB" node was added to the flow.A connection to an Astra DB instance was established.
A vector-enabled collection was created.

RAG Implementation – FAQ Handling:

The agent was enabled to retrieve information from a PDF FAQ document.
"PDF Loader," "Text Splitter," and "Embeddings" nodes were implemented.
The PDF was processed, embeddings were created, and stored in Astra DB.
The LLM was configured to use retrieved context.

Specialized Tool Development – Order Lookup:

An agent was created specifically for order lookups.
Database query nodes were added.
SQL queries were written (or database connector nodes were used) to retrieve order details.
The output was formatted for user-friendly display.

Agent Orchestration – Manager Agent:
A manager agent was built to direct user queries.
A "Router" or "Agent Executor" node was added.
Rules or prompts were defined to guide the manager's decisions.
The manager was connected to the FAQ and order lookup tools.

API Integration – External Access:

The system was enabled to be accessed via an API.The Langflow API endpoint was obtained.API calls were tested with tools like curl or Python's requests.

User Interface – Streamlit Front End:

A user-friendly web interface was created.
A Streamlit application was developed.
Input fields and display areas were implemented.
API calls to the Langflow flow were integrated.

References:

# AI-Agent-using-RAG-Langflow-Multi-Agents-
Get Started with DataStax Langflow: https://dtsx.io/agents Checkout Langflow: https://dtsx.io/3VEPL6Z OpenAI API Key: https://platform.openai.com/api-keys Weighing RAG Results: https://medium.com/logspace/beyond-basic-rag-retrieval-weighting-86deb741f5cc  

📌 Table of Contents

-[Introduction](#introduction)
Introduction [#Introduction]

Demo

Inspiration

What It Does

How We Built It

Challenges We Faced

How to Run

Tech Stack

Team

🎯 Introduction

This project implements a chatbot using Hugging Face embeddings and integrates it with Jira to retrieve relevant ticket information. The indexed Jira data is stored in a Chroma vector database for efficient retrieval based on similarity scores.

🎥 Demo

🔗 Live Demo (if applicable)📹 Video Demo (if applicable)🖼️ Screenshots:



💡 Inspiration

The need to efficiently retrieve Jira ticket information inspired this project. Managing and searching through Jira tickets manually can be time-consuming, so this chatbot automates the retrieval process using AI-based embeddings.

⚙️ What It Does

Fetches Jira ticket data using JiraReader

Converts Jira tickets into LangChain document format

Stores indexed Jira data using ChromaDB

Retrieves relevant information using similarity-based search

🛠️ How We Built It

Used JiraReader to fetch Jira data

Converted the data into LangChain document format

Indexed the documents using ChromaDB

Integrated HuggingFaceEmbeddings for similarity-based retrieval

🚧 Challenges We Faced

Ensuring correct Jira API integration and authentication

Optimizing the similarity threshold for effective retrieval

Managing and storing large volumes of Jira ticket data efficiently

🏃 How to Run

Clone the repository

git clone <repo_url>
cd <repo_name>

Install dependencies

pip install requests llama-index langchain chromadb transformers

Update the Jira credentials in the script:

JIRA_BASE_URL = "deeptibbdit.atlassian.net"
JIRA_EMAIL = "deepti.bbdit@gmail.com"
JIRA_API_TOKEN = "Your_Jira_API_Token"

Run the script to fetch and index Jira data:

python chatbot.py

Query the retriever:

retriever.invoke("DB issue")

🏗️ Tech Stack

🔹 Backend: Python

🔹 Libraries: LangChain, ChromaDB, Hugging Face Transformers

🔹 API Integration: Jira API

👥 Team
Pilot-AI


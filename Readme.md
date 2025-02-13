# Project Overview

This repository contains various implementations of AI agents using the Groq model. The agents are built using the agno framework, and they leverage different configurations and functions to provide specific tasks such as summarizing financial data, fetching company information, and web searches.

## Key Components

### Files and Functionalities
#### .env

Contains environment variables, specifically the API key for the Groq model.

#### agent_teams.py

Defines multiple AI agents (Web Agent and Finance Agent) and combines them into a team to perform tasks like summarizing analyst recommendations and sharing the latest news.
Utilizes the Groq model, DuckDuckGo for web searches, and YFinanceTools for financial data.

#### finance_agent_with_custom_function.py

Defines a Finance Agent with a custom function 
get_company_symbol
 to fetch company symbols.
Utilizes the Groq model and YFinanceTools for gathering financial data and additional stock symbol mappings.

#### finance_agent.py

Similar to the previous finance agent script but without the custom function.
Focuses on summarizing and comparing analyst recommendations and fundamentals for specific stocks using the Groq model and YFinanceTools.

#### simple_groq_agent.py

A basic implementation of an AI agent using the Groq model.
Tasked with generating a short information piece about Grok.

#### requirements.txt
Lists the required Python packages: 

## Libraries Used

**agno**: A framework generally used for building AI agents, orchestrating models, and integrating various tools.

**groq**: A library interfacing with the Groq AI models, used for natural language processing and generation tasks.

**dotenv** : A library for loading environment variables from a .env file into the application.

**yfinance**: A Python library used to access financial data from Yahoo Finance, providing tools for fetching stock prices, analyst recommendations, company info, and fundamentals.

**duckduckgo-search**: A Python library to use DuckDuckGo's search engine for web searches, providing results without tracking user queries.

### Conclusion
This repository showcases the utility and flexibility of combining AI models with various tools to perform complex data aggregation and summarization tasks. The agno framework coupled with libraries like groq, yfinance, and dotenv facilitates building powerful AI agents for specific domains such as finance and web searching.


### Execution Step

```
pip install virtualenv

# Create the virtual environment
virtualenv --python=python3 venv

# Activate the env
source venv/bin/activate

# Install dependencies in the env
pip install -r requirements.txt

# Run the agent file
python <filename>

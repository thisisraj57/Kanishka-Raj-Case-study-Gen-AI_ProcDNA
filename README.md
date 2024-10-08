Medical Research GenAI Processor
A powerful AI-driven application that processes, analyzes, and summarizes complex medical research papers, extracting essential information on drugs, genes, proteins, and medical efficacy/safety metrics. The application is built with Streamlit and leverages Google’s Generative AI model to empower medical research.

Features
Data Preprocessing: Secure data ingestion and preprocessing to tokenize, clean, and standardize medical research text.
Generative AI Query Processing: Answers user queries based on processed medical documents.
Entity Extraction: Extracts key medical entities such as drugs, genes, and proteins, using regular expressions.
Privacy Guardrails: Redacts patient identifiers and dates to ensure compliance with privacy standards.
Evaluation Metrics: Calculates Entity Linking Accuracy, Summary Coherence, and Readability Score for assessing query results.
Data Export: Provides functionality to download session data for offline access.
Getting Started


1. Prerequisites
Python 3.8 or higher
Streamlit
LangChain
Google Generative AI
NLTK for tokenization and BLEU score calculation
Plotly for visualizing extracted entity counts

2. Install required packages:
streamlit==1.18.1
langchain==0.0.300
langchain-google-genai==0.0.3
nltk==3.7
plotly==5.13.0
faiss-cpu==1.7.2


3. Set up Google Generative AI API Key: Add your Google Generative AI API key directly in the application or securely through an environment variable.

4. Running the Code
To run this code, ensure that you are in an environment that supports Jupyter notebook commands (e.g., Google Colab or Jupyter Lab). Here are the steps:

Install Localtunnel: Make sure you have internet access and npm installed in your environment.
Run the Python Code: Execute the consolidated code in your notebook cell.
Access the Application: After running, localtunnel will provide a public URL. Use that URL to access your Streamlit application from any web browser.

Notes
Ensure that your app.py is functioning correctly before running this script.
You may need to adjust firewall or security settings if you're running this in a restricted environment.
If localtunnel fails or does not connect, consider using alternatives like ngrok for exposing your application.



Application Overview
The application interface is divided into several key sections:

Main Query Section: Users input queries to retrieve insights from stored medical documents.
Entity Extraction: Automatically extracts drugs, genes, proteins, and efficacy metrics.
Evaluation Metrics: Displays evaluation scores to validate the response quality.
Data Export: Option to download query and response data for record-keeping.

Key Components
Data Preprocessing Pipeline: Loads and processes text, performing tokenization, entity extraction, and content cleaning.
Generative AI Processing Engine: Embeddings are generated through Google Generative AI’s embedding model.
Responses are generated using the gemini-1.5-pro model, a tailored model for accurate and coherent answers to medical queries.
Knowledge Base Integration: Extracted entities are validated against a mock knowledge base to ensure accurate entity linking.
Result Storage and Retrieval: Query and response history are stored in session state for easy access, with a download option for offline analysis.


Future Enhancements
Integration with external medical knowledge bases for real-time data updates.
Enhanced entity recognition using advanced models like BERT.
Support for additional evaluation metrics for more comprehensive analysis.


Contact
Developed by: Kanishka Raj
Contact: +91-9612223176

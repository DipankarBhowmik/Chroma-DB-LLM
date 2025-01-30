# Enhancing Medical Report Findings with Retrieval-Augmented Generation (RAG): Integrating LLM Models and Chroma DB using the LangChain framework for searchable data.
A POC for RAG on medical pdf reports

## At first, collect the MRI scan PDF reports.
## Convert it to text.
## By regular expression, remove private data.
## Then using REGEX, capture the information fields.
## After that, convert to JSON.
## Followed by conversion of Chroma DB format.
## Then chunking the text.
## Use Hugging Face Embeddings (all-MiniLM-L6-v2).
## Followed by storing and saving the embeddings in ChromaDB.
## Thereafter, test the solution. 
## Followed by Quality check by text evaluation metrics.

All the above pipeline is given practically in pdf_retrival_ChDB_LLM.ipynb.
For details, follow medium.com
https://bhowmikd1984.medium.com/enhancing-medical-report-findings-with-retrieval-augmented-generation-rag-integrating-llm-models-7db3c478264b


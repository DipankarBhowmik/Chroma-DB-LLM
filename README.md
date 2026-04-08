# Enhancing Medical Report Findings with Retrieval-Augmented Generation (RAG): Integrating LLM Models and Chroma DB using the LangChain framework for searchable data.
A POC for RAG on medical pdf reports

1️⃣ Load MRI PDF Report 📄

The process starts by loading the medical MRI report in PDF format containing radiology findings and patient observations.

2️⃣ Extract Text 🔍

The PDF content is extracted into raw text so that it can be processed by NLP models.

3️⃣ Remove Sensitive Information 🔒

Patient identifiers are removed to maintain privacy and ensure safe processing.

4️⃣ Text Chunking / Preprocessing ✂️

The report text is divided into smaller chunks to improve embedding generation and retrieval efficiency.

5️⃣ Generate Embeddings 🧠

Each text chunk is converted into vector embeddings that capture semantic meaning.

6️⃣ Store in Vector Database 🗄️

The embeddings are stored for fast similarity-based retrieval.

7️⃣ User Query Input ❓

The user provides a query such as "Patient is not cooperative".

8️⃣ Retriever (Top-k Relevant Chunks) 🎯

The retriever searches the vector database and returns top-k most relevant chunks.

9️⃣ Retrieval Evaluation — Precision@k & Recall@k 📊

At this stage, retrieval quality is evaluated:

Precision@k measures how many of the retrieved top-k chunks are actually relevant.
Recall@k measures how many relevant chunks were successfully retrieved out of all possible relevant chunks.
Higher Precision@k means fewer irrelevant results, while higher Recall@k means better coverage of relevant information.
🔟 Pass Retrieved Context + Query 🔗

The retrieved chunks are combined with the user query to create the prompt.

1️⃣1️⃣ LLM Generation 🤖

The prompt is sent to the language model to generate a concise medical summary.

1️⃣2️⃣ Generate Medical Summary 🩺

The model outputs key abnormalities and limitations.

1️⃣3️⃣ Summary Evaluation Metrics 📈

The generated summary is evaluated using:

BLEU
ROUGE
METEOR
BERTScore
1️⃣4️⃣ Final Output ✅

The system returns:

Retrieved context
Generated summary
Precision@k and Recall@k
NLP evaluation scores
For details, follow medium.com
https://bhowmikd1984.medium.com/enhancing-medical-report-findings-with-retrieval-augmented-generation-rag-integrating-llm-models-7db3c478264b


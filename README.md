# RAG Cookbooks
This repository covers the top 10 effective RAG techniques, along with an evaluation part in Athina AI.
## Introduction to RAG
Large Language Models are trained on a fixed dataset, which limits their ability to handle private or recent information. They can sometimes "hallucinate", providing incorrect yet believable answers. Fine-tuning can help but it is expensive and not ideal for retraining again and again on new data. The Retrieval-Augmented Generation (RAG) framework addresses this issue by using external documents to improve the LLM's responses through in-context learning. RAG ensures that the information provided by the LLM is not only contextually relevant but also accurate and up-to-date.
There are four main components in RAG:

![final](https://github.com/user-attachments/assets/a5e961da-d39e-48a8-af92-98a316b7fcbf)

**Indexing:** Documents are first chunked, and embeddings of these chunks are generated. These embeddings are then indexed into a vector store.

**Retriever:** Finds the most relevant documents based on a user's query, using techniques like vector similarity from the vector store.

**Augment:** Combines the user query with the retrieved context into a prompt, ensuring the LLM has the information needed to generate accurate responses

**Generate:** The combined query and prompt are passed to the model, which generates a response that is then provided as the final output to the user.

These components of RAG allow the model to access up-to-date, accurate information and generate responses based on external knowledge. However, to ensure RAG systems are functioning effectively, it’s essential to evaluate their performance.

## RAG Evaluation
Evaluating RAG applications is important for understanding how well these pipelines work. We can see how effectively they combine information retrieval with generative models by checking their accuracy and relevance. This evaluation helps improve RAG applications in tasks like text summarization, chatbots, and question-answering. It also identifies areas for improvement, ensuring that these systems provide trustworthy responses as information changes. Overall, effective evaluation helps optimize performance and builds confidence in RAG applications for real-world use. These notebooks contain an end-to-end RAG implementation + RAG evaluation part in Athina AI.

![my copy thumbnails (5)](https://github.com/user-attachments/assets/ad08db10-65ea-4ddd-b06b-2217797c4ceb)

## RAG Techniques
Here are the details of all 10 RAG techniques covered in this repository.

| Technique                    | Tools                        | Description                                                       | Notebooks |
|---------------------------------|------------------------------|--------------------------------------------------------------|-----------|
| Naive RAG      | LangChain, Pinecone, Athina AI                    | Combines retrieved data with LLMs for simple and effective responses.| [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/athina-ai/cookbooks/blob/main/naive_rag.ipynb) |

https://github.com/user-attachments/assets/c6f17961-40a1-4cca-ab1f-2c8fa3d71a7a









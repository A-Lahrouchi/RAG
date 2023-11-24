# How is RAG generally used
RAG is a technique for augmenting LLM knowledge with additional, often private or real-time, data

Retrieval: Given a user input, relevant splits are retrieved from storage using a Retriever

Generation: A ChatModel / LLM produces an answer using a prompt that includes the question and the retrieved data
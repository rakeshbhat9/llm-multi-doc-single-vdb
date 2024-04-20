## Proof of Concept - 

### Can we use LLMs to query documents, covering different topics but stored in same vector db as seperate collections.

Steps:
1. Create a single instance of ChromaDB vector store with multiple collections each for a distinct topic. - Covered in load-data-into-vectordb.ipynb
3. Using langchain create a [LOTR](https://python.langchain.com/docs/integrations/retrievers/merger_retriever/) pointed to each collection.
4. Use various available [Contextual Retrievers](https://python.langchain.com/docs/modules/data_connection/retrievers/contextual_compression/) to get only relevant document from LOTR.
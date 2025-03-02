## Overview
This project demonstrates the integration of [Qdrant](https://qdrant.tech/) with [LangChain](https://python.langchain.com/) for building scalable vector search applications. 

## Requirements
Ensure Python 3.8+ is installed along with `qdrant-client`, `langchain`, `numpy`, `pandas`, and `jupyter`/`colab`.

- **Architecture & Setup Images**

1. Qdrant Architecture with Langchain:
   
   ![Image1](https://github.com/Abhinavcode13/qdrant_langchain/blob/main/Images/qdrant.png)

    1. User asks a question → LangChain processes it  
    2. Embedding model converts the question into a vector  
    3. Qdrant retrieves relevant facts using the vector  
    4. Retrieved facts + question sent to LLM for response  
    5. LLM generates an answer and returns it to the user

2. On-premise server deployment using `Docker`

   ![Image2](https://github.com/Abhinavcode13/qdrant_langchain/blob/main/Images/qdrant-3.png)
   
    The Qdrant container is actively running in Docker with the image qdrant/qdrant:latest, accessible on port 6333:6333.

3. Qdrant API `Status` Check

   ![Image3](https://github.com/Abhinavcode13/qdrant_langchain/blob/main/Images/qdrant-4.png)

   This image shows a successful response from Qdrant running on `localhost:6333`

5. Qdrant `Cloud` Cluster Deployment 
   
   ![Image4](https://github.com/Abhinavcode13/qdrant_langchain/blob/main/Images/qdrant-5-cloud.png)

   This is the Qdrant UI for cloud deployment, where users set up `API` keys, choose a cluster, and select the appropriate cloud provider for hosting.
   Note: Qdrant Cloud URL: `https://cloud.qdrant.io`
   

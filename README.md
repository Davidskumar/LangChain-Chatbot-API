# LangChain Chatbot API

This is a **Conversational AI Chatbot** built using **LangChain, Flask, and Hugging Face models**.  
It retrieves technical courses from [Brainlox](https://brainlox.com/courses/category/technical) and allows users to ask questions via an API.

## 🚀 Features
- **Extracts Data** from a website using LangChain URL loaders  
- **Stores Embeddings** in a vector database (ChromaDB)  
- **Conversational AI** using `Mistral 7B` or other LLMs  
- **Flask API** for user interactions  
- **Deployed with Ngrok** for public access

## **Google Colab Notebook**
👉 [Run the chatbot in Google Colab](https://colab.research.google.com/drive/1z9EyV4KQq37De3YZFhRYpLFDOY60fcDQ?usp=sharing)  

## 📌 Installation & Usage
1. Health Check
   
   Method: GET
   
   URL: https://your-ngrok-url.ngrok.io/health
   
   Response:
  {
    "status": "ready"
  }

2. Chat with the AI

   Method: POST

   URL: https://your-ngrok-url.ngrok.io/chat

   or /test_qa_chain or /test_model

   Headers:
   {
     "Content-Type": "application/json"
   }

   Request Body:
  {
  "message": "Tell me about technical courses."
  }

   Response:
  {
    "response": "Here’s a list of technical courses: Data Science, AI, Web Development..."
  }

## Sample Output Screenshot

Here’s an example of the chatbot's response:

![Chatbot Output](screenshots/chatbot_output.png)
![Chatbot Output](screenshots/chatbot_output.png)










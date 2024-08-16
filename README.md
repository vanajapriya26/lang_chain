## Streamlit Chatbot

### The chatbot that we will be building will have the following features:

* It will stream the response from the LLM as it is being generated.
* It will use LangChain to interact with the LLM.
* It will use Streamlit to create the front-end of the app.
* It will remember the chat history and show it to the use

## Description:
- This Streamlit code creates a simple chatbot application using Google Generative AI (specifically, the "gemini-1.5-flash" model). The application begins by setting up the page's configuration, 
   including a title and icon. When the app runs, it starts with an initial message from the AI ("Hello, I am a bot. How can I help you?").

- The chatbot interacts with the user by maintaining a chat history, which is stored in st.session_state. When the user inputs a message, it gets appended to the chat history as a HumanMessage.
  
- The app then constructs a response using a prompt template that includes the chat history and the user's current question. This prompt is passed through a LangChain pipeline, which processes it 
  with the Google Generative AI model to generate a response. The response is streamed back to the user, displayed in the chat interface, and also stored in the chat history as an AIMessage.

- This code provides a basic framework for a conversational AI system, enabling back-and-forth communication between a user and an AI assistant, while preserving the context of the conversation.

  

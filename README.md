# LangChain: Summarize Text From YouTube or Website

This application summarizes content from a YouTube video or website using **LangChain** and **Groq's Gemma-7b-It model**. The app provides a user-friendly interface built with **Streamlit** to generate summaries of up to 300 words.

## Features

- Summarize YouTube videos or website content.
- Uses Groq's API with the Gemma-7b-It language model for summarization.
- Simple, interactive interface using Streamlit.
- Input validation and error handling.

Groq API Key
You will need a valid Groq API Key to use this app. The API key will be used to interact with Groq's language mode

## Requirements
Install the required Python packages:

## App Flow
Input API Key and URL: The user inputs the Groq API key and provides a YouTube or website URL for summarization.

Validation: The app validates the API key and URL format before processing.

Content Loading:
If the URL is from YouTube, the app extracts the video content using YoutubeLoader.

If the URL is from a website, the content is loaded using UnstructuredURLLoader.

Summarization: The content is summarized using the Groq model and displayed in the app.

## Error Handling
The app checks if all inputs are provided.

It validates whether the URL is in the correct format.

Any unexpected errors will be shown in the Streamlit app with a detailed message.

```bash
pip install streamlit validators langchain langchain_groq langchain_community

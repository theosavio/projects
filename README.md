# Video Analytics using Vertex AI

This project utilizes Vertex AI and various libraries to perform video analytics, including question answering based on the text content of the video.

## Setup

1. Install required dependencies:
   ```bash
   pip install google-cloud-aiplatform langchain chromadb pytube youtube-transcript-api gradio
1.authenticate with google cloud

from google.colab import auth as google_auth
google_auth.authenticate_user()

2.Initialize Vertex AI:

import vertexai
PROJECT_ID = "<your-project-id>"
vertexai.init(project=PROJECT_ID)

## Usage

1.Load video data:
Use the YoutubeLoader to load video content from a YouTube URL.

2.Split text content:
Split the text content of the video into smaller documents using RecursiveCharacterTextSplitter.

3.Create ChromaDB:
Create a ChromaDB from the text documents for efficient search.

4.Question Answering:
Use the sm_ask function to ask questions based on the video content and get responses.

5.Gradio Interface:
Launch a Gradio interface to interactively ask questions and get responses.

## Contributing

Contributions are welcome! If you have ideas for improvements or new features, feel free to open an issue or submit a pull request.

## Resources
Google Cloud AI Platform Documentation
Langchain Documentation
ChromaDB Documentation
PyTube Documentation
YouTube Transcript API Documentation
Gradio Documentation

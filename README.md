# Building Multimodal LLM Applications

This project demonstrates how to build generative AI applications for multimodal tasks using OpenAI and LangChain.  
It transcribes text from a video or audio file and allows users to ask context-aware questions about the transcribed content using a chat model.

## Overview

The project integrates multiple modalities — audio and text — into a single workflow.  
It uses OpenAI’s transcription model to convert speech into text and LangChain’s conversational interface to reason over the text.  

All tasks, including downloading videos, extracting audio, transcribing, and querying text, are implemented and demonstrated in the Datalab/Datacamp **notebook**, which serves as the main interface for experimentation and exploration.  

**Ethical Data Use:**  
All video and audio content used in this project is sourced from the [Internet Archive](https://archive.org/) under free licenses, ensuring ethical and legal data access.

This project is intended for developers who want to explore practical implementations of multimodal large language models (LLMs) and build intelligent systems that understand both audio and text data.

## Key Features

- Automatic speech-to-text transcription using OpenAI.
- Contextual question-answering using LangChain and OpenAI chat models.
- Modular pipeline integrating audio processing, transcription, and LLM interaction.
- Implemented in a notebook for step-by-step demonstration.
- Compatible with local files or online video/audio links.
- Lightweight, easy to extend, and developer-friendly.

## Tech Stack

- OpenAI API (`gpt-4o-mini`, `gpt-4o-mini-transcribe`)  
- LangChain  
- Python 3.8+  
- `pydub` for audio handling  
- `yt-dlp` for downloading and extracting audio  
- Datalab / DataCamp Notebook environment  
- Git and GitHub for version control  

## Project Structure
files/
├── audio/ # Stores extracted or uploaded audio files
├── transcripts/ # Stores transcription outputs
├── notebook.ipynb # Datalab notebook where the project workflow is implemented
└── requirements.txt # Dependency file

## Setup and Installation

1. Clone the repository: 

  ```bash
   git clone https://github.com/your-username/Multimodal-LLMs-With-Langchain-OpenAI.git

2. Navigate into the project directory:

cd Multimodal-LLMs-With-Langchain-OpenAI

3. Install dependencies:

pip install -r requirements.txt

4. Add your OpenAI API key as an environment variable:

openai_api_key = os.getenv("OPENAI_API_KEY")

5. Open the notebook (notebook.ipynb) to run the workflow interactively.

## Usage Example

Provide a video or audio file (from Internet Archive or local source).

The notebook extracts audio (if necessary) and transcribes it using OpenAI’s model.

After transcription, the text can be queried interactively using a chat model through LangChain.

Example:

User: "What was the main topic discussed in the video?"

Assistant: "The speaker focused on the importance of multimodal systems and their role in AI understanding."

## Contribution

Developers are welcome to contribute improvements, such as better error handling, UI integration, or extending the pipeline to handle image inputs.

## License

This project is open for educational and experimental use.


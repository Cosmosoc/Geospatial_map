# Voice Recognition Geospatial Map

This FastAPI project provides a speech-to-text transcription service, coupled with natural language processing to identify commands, locations, and map types from audio files.

## Table of Contents
- [Installation](#installation)
- [Dependencies](#dependencies)
- [Running the API](#running-the-api)
- [Environment Variables](#environment-variables)

## Installation

Clone this repository and install the required packages using the following command.

### Dependencies

The following dependencies are necessary for different functionalities in the project:

- **FastAPI**: A modern web framework for building APIs with Python 3.7+ that is easy to use, fast, and asynchronous. It will handle the API endpoints.
  
- **Uvicorn**: An ASGI server used to run the FastAPI application for asynchronous server communication.

- **PyTorch (torch)**: A deep learning framework that provides tools for creating and running machine learning models, required for speech-to-text processing and NLP tasks.

- **Transformers**: A library by Hugging Face that provides pre-trained models for various natural language processing (NLP) tasks, including automatic speech recognition (ASR) and other NLP pipelines.

- **SoundFile**: A library for reading and writing audio files in different formats, essential for handling input audio files in the API.

- **NumPy**: A fundamental package for scientific computing in Python, used for array handling and numerical operations in various parts of the application.

- **ffmpeg-python**: A wrapper for FFmpeg, allowing you to convert audio files between different formats (e.g., WAV, MP3) to ensure compatibility with your ASR models.

- **python-dotenv**: This library helps load environment variables from a `.env` file, allowing you to store sensitive information like API keys securely.

- **OpenCage Geocoder (opencage)**: A library to convert place names or addresses into geographic coordinates (latitude/longitude), which is used to geocode locations from the user's spoken input.

- **NLTK**: The Natural Language Toolkit provides various resources and tools for text processing tasks like tokenization, stemming, and stopword removal.

- **scikit-learn**: A machine learning library used for tasks such as cosine similarity calculations to match spoken commands with stored geographic data.

- **Sentence-Transformers**: A library that allows semantic similarity matching of sentences, used to match spoken commands to predefined map-related actions.

- **pydub**: A Python library for audio data manipulation tasks, used for various audio processing needs such as format conversion or splitting.

After installing NLTK, remember to download the necessary stopwords dataset by running the following in a Python shell:

import nltk
nltk.download('stopwords')
  

### Install the Dependencies

You can install all the necessary dependencies in one go by running the following command:

```bash
# Install dependencies
pip install fastapi "uvicorn[standard]" torch transformers soundfile numpy ffmpeg-python python-dotenv opencage nltk scikit-learn sentence-transformers pydub

# Voice Recognition Geospatial map

This FastAPI project provides a speech-to-text transcription service, coupled with natural language processing to identify commands, locations, and map types from audio files.

## Table of Contents
- [Installation](#installation)
- [Dependencies](#dependencies)
- [Running the API](#running-the-api)
- [Environment Variables](#environment-variables)

## Installation

Clone this repository and install the required packages as listed below.

### Dependencies

Install each package with the following commands:

```bash
# FastAPI - For building the API server.
pip install fastapi

# Uvicorn - For running the FastAPI application.
pip install "uvicorn[standard]"

# PyTorch (torch) - Required for loading and running deep learning models.
pip install torch

# Transformers - Hugging Face Transformers library for ASR and NLP models.
pip install transformers

# SoundFile - For reading and writing audio files in various formats.
pip install soundfile

# NumPy - For handling arrays and numerical data processing.
pip install numpy

# ffmpeg-python - For handling audio format conversions.
pip install ffmpeg-python

# python-dotenv - For loading environment variables from a .env file.
pip install python-dotenv

# OpenCage Geocoder (opencage) - For geocoding locations using the OpenCage API.
pip install opencage

# NLTK - Natural Language Toolkit for NLP preprocessing.
pip install nltk

# After installing NLTK, download stopwords in a Python shell
# (necessary for text processing).
import nltk
nltk.download('stopwords')

# scikit-learn - For cosine similarity calculations in text processing.
pip install scikit-learn

# Sentence-Transformers - For semantic similarity matching of commands.
pip install sentence-transformers

# pydub - For handling audio data manipulation tasks.
pip install pydub

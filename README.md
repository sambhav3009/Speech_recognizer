# Speech Recognizer 🎤➡️📝

This is a Python project that converts spoken audio into text. The program processes audio files by splitting them into manageable chunks and then uses speech recognition to transcribe the audio into written text. This can be beneficial for applications requiring transcription services or for users who need to convert audio content into a readable format.

## Table of Contents
- [Features](#features)
- [How It Works](#how-it-works)
- [Requirements](#requirements)


## Features

- Converts audio files from MP3 to WAV format.
- Splits large audio files into chunks based on silence to enhance transcription accuracy.
- Utilizes Google Speech Recognition API for converting speech to text.
- Exports transcribed text for further use.

## How It Works

1. **Audio Conversion**: 
   - The program uses `ffmpeg` to convert audio files from MP3 to WAV format, which is more suitable for processing.
2. **Chunking the Audio**: 
   - The audio is divided into smaller chunks where silence is detected, allowing for easier processing and recognition.
3. **Speech Recognition**: 
   - Each audio chunk is processed using the `SpeechRecognition` library to convert the speech into text.
4. **Text Compilation**:
   - The transcribed text from each chunk is combined into a single output text.

## Requirements

- Python 3.x
- Install the following packages:

   ```bash
   pip install SpeechRecognition pydub
   sudo apt install ffmpeg

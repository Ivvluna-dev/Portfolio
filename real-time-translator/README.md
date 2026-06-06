# Real-Time Translator

## Overview

Real-Time Translator is a Python application that captures live audio, transcribes spoken English speech and translates it into Spanish in real time.

The project was created as a learning experience to improve my programming, debugging and software development skills while working with audio processing, machine learning models and desktop application development.

## Features

* Real-time audio capture
* Microphone and system audio (loopback) support
* Automatic audio device selection
* Speech-to-text transcription using OpenAI Whisper
* English to Spanish translation
* On-screen subtitle overlay
* Low-latency processing pipeline
* System tray integration

## Technologies Used

* Python
* OpenAI Whisper
* PyTorch
* Hugging Face Transformers
* PyQt5
* NumPy
* SoundDevice
* SoundCard

## How It Works

The application captures audio from either a microphone or system output.

The audio is processed through a multi-threaded pipeline:

1. Audio Capture
2. Voice Detection
3. Speech Transcription
4. Translation
5. Subtitle Display

The translated text is displayed in a transparent overlay window directly on screen.

## Skills Demonstrated

* Python Programming
* Debugging and Troubleshooting
* Audio Processing
* Multithreading
* Machine Learning Integration
* Desktop Application Development
* User Interface Design
* Technical Documentation
* AI-Assisted Development Workflows

## Challenges Solved

During development, several technical challenges were addressed, including:

* Audio device detection
* Loopback audio capture
* Translation latency optimization
* Duplicate transcription filtering
* Real-time subtitle rendering
* Performance optimization for CPU and GPU environments

## Project Status

Work in Progress

The application is actively being improved with new features, optimizations and usability enhancements.

## Learning Outcomes

This project helped me gain practical experience with Python, software architecture, debugging, audio processing, machine learning models and real-world application development.

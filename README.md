# Audio Transcription Project with Avatar Lip-Syncing

This project implements a real-time audio transcription solution using the **Whisper** model and **torchaudio**, with support for English and Arabic language detection. The transcription is performed on incoming audio, converting spoken words into text. Additionally, the project integrates **Wav2Lip** to generate a video where an avatar lip-syncs to the transcribed speech. The system has been optimized to process video efficiently, ensuring timely avatar responses, and includes an interactive **Gradio** interface for easy user interaction.

## Key Features:
- **Real-time Audio Transcription**: Using the Whisper model, the system transcribes both English and Arabic speech into text.
- **Language Detection**: Automatically detects whether the input audio is in English or Arabic and adjusts transcription accordingly.
- **Avatar Lip-Syncing**: Generates a video of an avatar that lip-syncs with the transcribed audio using the Wav2Lip model.
- **Optimized Video Processing**: The video processing time has been optimized for faster performance.
- **Gradio Interface**: Provides a user-friendly interface for uploading audio, processing it in real-time, and viewing the lip-synced avatar video.

## Components:
1. **Whisper Model for Transcription**: Whisper is a state-of-the-art speech recognition model that supports multilingual transcription, making it ideal for both English and Arabic audio.
2. **Torchaudio for Audio Handling**: Utilized for handling and preprocessing the audio input before feeding it into the transcription model.
3. **Wav2Lip for Lip-Syncing**: The Wav2Lip model is responsible for generating lip-sync videos, ensuring accurate synchronization of the avatar’s lips with the transcribed speech.
4. **Gradio Interface**: Gradio provides an easy-to-use interface for users to interact with the transcription and lip-syncing system. Users can upload audio files, transcribe them, and view the avatar video output.

## Workflow:
1. **Audio Input**: Users upload an audio file (in English or Arabic) through the Gradio interface.
2. **Language Detection**: The system detects the language of the audio input.
3. **Audio Transcription**: The Whisper model transcribes the speech into text based on the detected language.
4. **Lip-Sync Video Generation**: Wav2Lip generates a video where the avatar lip-syncs with the transcribed audio.
5. **Optimization**: Video processing time has been optimized to ensure minimal delays during generation.
6. **Output**: The Gradio interface displays the transcribed text and the lip-sync video for the user.

## Benefits:
- **Real-time Processing**: Provides fast audio transcription and video generation, ideal for interactive use cases.
- **Multilingual Support**: Seamlessly handles both English and Arabic audio input.
- **User-Friendly**: With the addition of the Gradio interface, the system is accessible to users with minimal technical expertise.

# Project Overview

The project consists of two main parts:

**RealTimeVoiceRec Notebook:**

In this notebook, you can record audio in real-time and transcribe it.
This is useful for scenarios where you need to capture the audio on the fly.


**RealTimeVoiceFinal Notebook:**

In this notebook, you can manually upload an audio file for transcription.
This option is ideal when you already have audio files and want to transcribe them.

**RealTimeVoiceRecFinal(eng_and_ara)_.(FINALLL) Notebook:(Final Update)**

This Notebook is a powerful voice recognition tool that supports both English and Arabic speech, utilizing advanced neural network technology from Neural Space for Text-to-Speech (TTS) capabilities, dynamically detecting and processing the language of audio recorded by the user, and features a simple Gradio interface for easy interaction.


# How It Works


Language Detection: The system detects whether the audio is in English or Arabic based on a snippet of the audio.
Audio Processing: The audio file is processed to ensure it's in the correct format (mono and 16kHz sample rate).
Transcription: Using the Whisper model, the audio is transcribed into text, with the correct language token applied.
Lip-Syncing: The transcribed audio can then be applied to a video of an avatar, which uses Wav2Lip to lip-sync the spoken words, creating a realistic talking avatar.


# Usage

**RealTimeVoiceRec (Real-Time Recording)**


Run the notebook RealTimeVoiceRec.
Use the record_audio function to capture audio directly from your microphone.
The notebook will detect the language and transcribe the recorded audio.
Apply the transcription to an avatar video using Wav2Lip to create a lip-synced video.


**RealTimeVoiceFinal (Manual Audio Input)**

Run the notebook RealTimeVoiceFinal.
Upload an existing audio file (.wav format).
The notebook will process the uploaded file, detect the language, and generate a transcription.
Use the transcribed audio to create a lip-synced avatar video with Wav2Lip.


# Requirements
To run this project, you will need:

Python 3.x
torchaudio
torch
transformers library (for the Whisper model)
Wav2Lip for avatar lip-syncing
(Optional) pyaudio if you're using the real-time recording functionality


*Install the necessary packages using:*

pip install torchaudio torch transformers



# Here's how you can use the project

Record or upload an audio file.
Run the transcription function to generate the text.
Use the Wav2Lip model to lip-sync the avatar video with the transcribed audio.
The final result will be a video of the avatar talking.


**Future Enhancements**
Improve the language detection with a more advanced model.
Support additional languages and transcription formats.
Enhance the avatar customization options for a more personalized experience




# Audio Transcription Project with Avatar Lip-Syncing

This project provides a simple solution for real-time audio transcription using the Whisper model and torchaudio. It detects the language of the audio input (supports English and Arabic) and transcribes the speech into text. Additionally, the transcribed audio can be used to create a video of an avatar that lip-syncs the spoken words using Wav2Lip.

# Project Overview

The project consists of two main parts:

**RealTimeVoiceRec Notebook:**

In this notebook, you can record audio in real-time and transcribe it.
This is useful for scenarios where you need to capture the audio on the fly.


**RealTimeVoiceFinal Notebook:**

In this notebook, you can manually upload an audio file for transcription.
This option is ideal when you already have audio files and want to transcribe them.


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


**License**
This project is licensed under the MIT License - see the LICENSE file for details.

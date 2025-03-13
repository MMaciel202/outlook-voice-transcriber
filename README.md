#Outlook Voice Transcriber

#Overview

This Python script automatically processes voicemail messages received via Outlook email, transcribes the audio using OpenAI Whisper, and sends the transcription back to the original recipient via email.

Features
•	Fetches emails from Outlook.
•	Extracts and saves audio attachments.
•	Transcribes audio using Whisper.
•	Sends transcription back to the original recipient.

Prerequisites
•	The telephone system must be configured to send audio messages to your inbox.
•	Python 3.8+
•	Microsoft Outlook installed (for email access via COM interface)
•	Required Python libraries: 
   o	whisper
   o	win32com.client
   o	os
   o	getpass
•	FFmpeg is included in the repository, so no external installation is required.

Installation
1. Clone the Repository

   To get the repository, run:
   git clone https://github.com/yourusername/outlook-voice-transcriber.git
   cd outlook-voice-transcriber
   
2. Create a Virtual Environment (Recommended)
   
   To avoid dependency conflicts, create a virtual environment:
   •	Windows: 
   •	python -m venv venv
   •	venv\Scripts\activate
   •	MacOS/Linux: 
   •	python3 -m venv venv
   •	source venv/bin/activate

   After activation, your terminal should show (venv) before the command prompt.

3. Install Dependencies
   
   First, ensure pip is up to date:

   pip install --upgrade pip
   
   Then, install the required dependencies:

   pip install -r requirements.txt
   
Configuration

•	To change the sender's email address, edit the transcriber.py file and modify the SENDER_EMAIL variable at the top of the script: 
•	SENDER_EMAIL = "your_sender_email@example.com".lower()
•	Ensure the script has access to Outlook emails.

Usage
Run the script with:
python transcriber.py

Notes
•	Ensure Outlook is running and properly configured.
•	Whisper may take some time to process large audio files.

License
This project is licensed under the MIT License.
    
      


    
    
   

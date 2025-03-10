# outlook-voice-transcriber
This script automatically transcribes voicemail messages received via Outlook email.

# How to Clone, Install, and Run Transcriber
This guide will walk you through cloning the repository, installing dependencies, setting up a virtual environment, and running the Trabscriber script.

1. Cloning the Repository
   To get the repository
   git clone https://github.com/MMaciel202/outlook-voice-transcriber.git
   cd outlook-voice-transcriber

2. Creating a Virtual Environment
   It's recommended to use a virtual environment to avoid dependency conflicts.

   - Windows:
     python -m venv venv
     venv\Scripts\activate
     
   - MacOS/Linux:
     python3 -m venv venv
     source venv/bin/activate
  After activation, your terminal should show (venv) before the command prompt.

3.  Installing Dependencies
    First, make sure you have pip up to date:
    pip install --upgrade pip
    Then, install the required dependencies:
    pip install -r requirements.txt

4.  Install FFmpeg (Required for Audio Processing)
    The script depends on FFmpeg for audio conversion. Install it as follows:

    - Windows: Download and install FFmpeg from the FFmpeg official site and add it to your system PATH.
    - Linux: Install via package manager: sudo apt install ffmpeg #Debian/Ubuntu
    - macOS: brew install ffmpeg #macOS (Homebrew)

5.  Run the Script
    After installing all dependencies, run the script with:
    python transcriber.py

    
      


    
    
   

# InsightSage - AI-Powered Meeting Assistant

InsightSage is an advanced meeting assistant that transforms audio recordings into actionable insights, task assignments, and interactive summaries. Built with cutting-edge AI technology, it streamlines the meeting workflow from transcription to task management.

## 🌟 Features

- **Audio Processing**
  - MP3 to WAV conversion
  - High-quality audio transcription
  - Speaker diarization
  - Multi-format transcript generation (TXT & JSON)

- **AI-Powered Analysis**
  - Intelligent meeting summarization
  - Automated task extraction
  - Customizable AI agent for task identification
  - Interactive Q&A about meeting content

- **Task Management**
  - Automated task assignment
  - Email notifications with customizable templates
  - Deadline tracking
  - Participant management

- **User Interface**
  - Modern, animated gradient design
  - Real-time progress tracking
  - Interactive chat interface
  - File browser and diagnostics

## 🛠️ Technology Stack

- **Frontend**: Streamlit
- **AI/ML**: 
  - LangChain
  - Ollama (deepseek-r1:1.5b model)
  - Whisper (for transcription)
- **Audio Processing**: FFmpeg
- **Email**: SMTP (Gmail)
- **File Formats**: MP3, WAV, TXT, JSON

## 📋 Prerequisites

- Python 3.8+
- FFmpeg installed
- Ollama installed with deepseek-r1:1.5b model
- Gmail account (for email notifications)

## 🚀 Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/InsightSage.git
cd InsightSage
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. Set up FFmpeg:
   - Download FFmpeg from the official website
   - Place it in the project directory under `ffmpeg-master-latest-win64-gpl-shared`

4. Set up Ollama:
```bash
ollama pull deepseek-r1:1.5b
```

5. Set up environment variables:
   - Copy `.env.example` to `.env`
   - Add your HuggingFace token and email credentials
   - Never commit the `.env` file to version control

## 💻 Usage

1. Start the application:
```bash
streamlit run new_app.py
```

2. Upload an MP3 file through the interface

3. Configure email settings in the sidebar (optional)

4. Use the AI agent for task extraction (optional)

5. View transcripts and summaries

6. Send task assignments via email

## 📁 Project Structure

```
InsightSage/
├── Audio/                 # Uploaded MP3 files
├── WAV_Audio/            # Converted WAV files
├── TEXT_Transcripts/     # Text format transcripts
├── JSON_Transcripts/     # JSON format transcripts
├── Summaries/           # Generated meeting summaries
├── ffmpeg-master-latest-win64-gpl-shared/  # FFmpeg installation
├── new_app.py           # Main application file
├── audio_transcription.py  # Audio transcription script
├── process_transcripts.py  # Transcript processing script
├── mp3_to_wav.py        # MP3 to WAV conversion script
└── requirements.txt     # Python dependencies
```

## 🔧 Configuration

### Email Settings
Configure email settings in the sidebar:
- Email sender address
- Email password (Gmail app password)
- Custom email template

### AI Agent Settings
Customize the AI agent behavior:
- Model selection
- Temperature adjustment
- Custom extraction prompts

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- FFmpeg for audio processing
- Ollama for AI capabilities
- Streamlit for the web interface

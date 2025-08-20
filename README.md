# CHAOS AI Assistant 🤖

A powerful voice-activated AI assistant built with Python that combines Google Gemini AI, Spotify integration, and system control capabilities.

## ✨ Features

- **Voice Recognition**: Speak naturally to control your computer
- **AI Conversations**: Powered by Google Gemini 1.5 Flash
- **Music Control**: Play songs directly from Spotify
- **System Control**: Manage applications, volume, and system functions
- **Web Navigation**: Open websites and perform web searches
- **Persistent Memory**: Remembers conversation context
- **Text-to-Speech**: Natural voice responses

## 🎯 Capabilities

### 🗣️ Voice Commands
- "Play [song name]" - Play music from Spotify
- "Open [website/application]" - Launch apps or websites
- "Close [application]" - Terminate running applications
- "Search for [query] on the browser" - Web search
- "What's the time?" - Get current time
- "Increase/decrease volume" - Control system volume
- "Shutdown/restart" - System control

### 💬 AI Chat
- Natural conversation with context memory
- Task assistance and general queries
- Conversation history persistence

## 🚀 Installation

### Prerequisites
- Python 3.7 or higher
- Windows OS (for system control features)
- Microphone for voice input
- Spotify Premium account (for music features)

### Setup Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/chaos-ai-assistant.git
   cd chaos-ai-assistant
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure API Keys**
   ```bash
   cp config_template.py config.py
   ```
   
   Edit `config.py` with your API credentials:
   - Google Gemini API key
   - Spotify Client ID and Secret

4. **Run the assistant**
   ```bash
   python final.py
   ```

## 🔧 Configuration

### Required API Keys

#### Google Gemini API
1. Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Create a new API key
3. Add to `config.py` as `apikey`

#### Spotify API
1. Go to [Spotify Developer Dashboard](https://developer.spotify.com/dashboard)
2. Create a new app
3. Get Client ID and Client Secret
4. Add to `config.py`

### Configuration Options

Edit `config.py` to customize:
- TTS voice and speech rate
- Audio timeout settings
- File paths for logs and memory

## 📖 Usage

### Text Mode
```
Welcome to CHAOS AI! Type 'exit' to quit or say 'exit' during audio input.
Type your command or say 'audio' for voice input:
> play despacito
```

### Voice Mode
```
> audio
CHAOS: Listening for up to 5 seconds.
You said: play despacito
CHAOS: Playing Despacito by Luis Fonsi.
```

## 🎵 Spotify Setup

1. Install Spotify on your device
2. Log in to your Spotify Premium account
3. Keep Spotify running for music playback
4. First-time use will require authentication

## 📁 Project Structure

```
chaos-ai-assistant/
├── final.py                 # Main application
├── config_template.py       # Configuration template
├── requirements.txt         # Dependencies
├── README.md               # This file
├── .gitignore              # Git ignore rules
└── chat_memory.json        # Conversation history (auto-generated)
```

## 🛡️ Security Notes

- Never commit `config.py` to version control
- API keys are stored locally only
- Conversation logs are stored locally
- Use environment variables for production deployment

## 🚨 Troubleshooting

### Common Issues

**"config.py not found!"**
- Copy `config_template.py` to `config.py`
- Add your API keys to the new file

**Speech recognition not working**
- Check microphone permissions
- Install pyaudio: `pip install pyaudio`
- On Windows, you might need Microsoft Visual C++ 14.0

**Spotify not playing**
- Ensure Spotify Premium account
- Keep Spotify app running
- Check device availability in Spotify

**Voice not working**
- Install speech engines: `pip install pyttsx3`
- Try different voice indices in config

## 🔄 Updates

Check the [CHANGELOG.md](CHANGELOG.md) for version updates and new features.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

## 📞 Support

If you encounter issues or have questions:
- Open an issue on GitHub
- Check the troubleshooting section
- Review the configuration template

## ⚠️ Disclaimer

This software is for educational and personal use. Be cautious with system control features and ensure you have proper permissions for all integrations.

---

**Made with ❤️ by [Your Name]**

*CHAOS AI - Bringing order to your digital chaos!*

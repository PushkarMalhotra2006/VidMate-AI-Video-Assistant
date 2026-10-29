# 🎬 VidMate — AI Video Assistant

**Turn videos into knowledge with AI.**

VidMate is an AI-powered video assistant that transforms video content into useful information. It transcribes audio, generates summaries and notes, and allows users to ask questions about video content through a Retrieval-Augmented Generation (RAG) chatbot.

---

## ✨ Features

- 🎥 **Video Input:** Process videos using YouTube URLs or upload local video files.
- 📝 **Automatic Transcription:** Convert spoken content into text using speech recognition.
- 📄 **AI-Powered Summarization:** Generate concise summaries of video content.
- 📚 **Smart Notes:** Extract important information for revision and reference.
- 💬 **AI Chatbot:** Ask questions about the processed video and receive context-based answers.
- 🔎 **RAG-Based Retrieval:** Retrieve relevant information from video transcripts to help answer user questions.
- 🖥️ **Interactive Interface:** Access the application's features through a Streamlit interface.

---

## 🛠️ Tech Stack

- **Language:** Python
- **Frontend:** Streamlit
- **Speech Recognition:** faster-whisper
- **Audio Processing:** FFmpeg, pydub
- **LLM Orchestration:** LangChain
- **Vector Database:** ChromaDB
- **Embeddings:** Sentence Transformers
- **LLM Providers:** Google Gemini, Groq
- **Video Downloading:** yt-dlp

---

## ⚙️ How It Works

1. **Video Input:** Provide a YouTube URL or upload a local video file.
2. **Audio Processing:** Extract and process the video's audio.
3. **Transcription:** Convert the audio into text using speech recognition.
4. **Summarization:** Generate a concise summary of the video using an LLM.
5. **Note Generation:** Create useful notes from the video content.
6. **Vector Storage:** Split the transcript into chunks, generate embeddings, and store them in a vector database.
7. **Question Answering:** Ask questions through the chatbot, which retrieves relevant transcript chunks to generate context-based answers.

---

## 📂 Project Structure

```text
VidMate - AI Video Assistant/
│
├── core/
│   ├── notes.py              # Generates notes from video content
│   ├── rag_engine.py         # RAG-based question-answering engine
│   ├── summarizer.py         # Generates video summaries
│   ├── transcribe.py         # Transcribes video audio
│   └── vector_store.py       # Manages vector storage and retrieval
│
├── utils/
│   └── audio_processing.py   # Audio extraction and processing utilities
│
├── app.py                    # Streamlit user interface
├── main.py                   # Main video processing pipeline
├── requirements.txt          # Project dependencies
├── .env                      # Environment variables (not committed)
├── .gitignore                # Git exclusions
├── .gitattributes            # Git attributes configuration
└── README.md                 # Project documentation
```

---

## 💡 Use Cases

- **Students:** Summarize lectures and generate revision notes.
- **Researchers:** Extract key information from educational videos.
- **Developers:** Quickly review technical tutorials.
- **Content Consumers:** Ask questions about videos without manually searching through the entire content.

---

## ⚠️ Limitations

- Transcription accuracy depends on audio quality and the speech recognition model.
- Processing time varies depending on video length, hardware, and model configuration.
- AI-generated summaries and answers may occasionally omit details or contain inaccuracies.
- YouTube URL processing may be affected by video availability and platform restrictions.
- LLM features may require API keys and may be subject to provider quotas or usage costs.

---

## 👨‍💻 Author

Pushkar Malhotra
**Pushkar Malhotra**

GitHub: [PushkarMalhotra2006](https://github.com/PushkarMalhotra2006)

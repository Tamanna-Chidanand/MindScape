# MindScape
MindScape is a dynamic, AI-driven text-based adventure game that uses large language models and multimodal AI to generate personalized, real-time narratives. By combining storytelling with generative AI, it enables players to interact with adaptive characters and evolving storylines enhanced with visuals.

## 📜 Abstract

Conventional text-based games often rely on static, pre-written narratives. MindScape reimagines this genre by using **Retrieval-Augmented Generation (RAG)**, **HuggingFace Transformers**, and **local language models** to create coherent and immersive storylines in real time. The system also includes **text-to-image** and **text-to-speech** synthesis for deeper immersion.

## Features

- Real-time interactive storytelling with LLMs  
- AI-generated visuals using Replicate's Flux-Schnell model  
- Audio narration via text-to-speech synthesis  
- Memory-augmented context retrieval with ChromaDB  
- Dynamic player choices influencing game flow  
- Save/load functionality for persistent gameplay  
- Web-based interface built with FastAPI  

## System Architecture

- **Frontend**: React.js (user interface)  
- **Backend**: FastAPI (Python)  
- **Game Engine**: Handles player decisions, story progression  
- **LLM Interface**: Connects to models like OPT-350M, LLaMA, Ollama  
- **Vector Store**: ChromaDB for semantic search and retrieval  
- **Visual Engine**: Replicate API for fantasy artwork generation  
- **Audio Engine**: Text-to-speech module (future extensible)  

## Tech Stack

| Component        | Technology                            |
|------------------|----------------------------------------|
| Backend          | Python, FastAPI, Uvicorn, Pydantic     |
| Frontend         | React.js                               |
| LLMs             | OPT-350M, LLaMA, Ollama                |
| Embeddings       | Sentence Transformers (MiniLM-L6-v2)   |
| Vector DB        | ChromaDB                               |
| Text-to-Image    | Replicate API (Flux-Schnell)           |
| Deployment       | Docker (optional), localhost           |

## Running Locally

### 1. Clone the repository
git clone https://github.com/<your-username>/mindscape.git
cd mindscape
`

### 2. Set up Python environment
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
pip install -r requirements.txt


### 3. Start the backend server
uvicorn main:app --reload


### 4. Start the frontend (if applicable)
cd frontend
npm install
npm start


## Results

- Improved narrative coherence through RAG-based context  
- High replayability due to procedural content  
- Enhanced user engagement with multimodal feedback  

## Future Enhancements

- Multiplayer storytelling support  
- Emotion-aware text-to-speech  
- 3D visual generation and VR integration  
- Procedural character and quest generation  
- Bias mitigation and ethical AI narratives  

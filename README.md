# ai-film-factory
AI Film Factory is a modular production system that transforms raw scripts into fully rendered cinematic sequences using automation, generative AI, and real-time pipelines.
# 🎬 AI Film Factory
### End-to-End AI Cinematic Production Pipeline

> Script → Shotlist → Prompts → Generation → Edit → Final Render

AI Film Factory is a modular production system that transforms raw scripts into fully rendered cinematic sequences using automation, generative AI, and real-time pipelines.

---

## 🔥 Why This Exists

Traditional video production is slow, expensive, and fragmented.

AI Film Factory compresses the pipeline into a **single automated system**, enabling:
- ⚡ Rapid content generation
- 🎯 Consistent visual storytelling
- 💰 Massive cost reduction
- 🔁 Scalable iteration loops

---

## 🧠 System Architecture
         ┌────────────────────┐
         │     SCRIPT INPUT    │
         └─────────┬──────────┘
                   ↓
         ┌────────────────────┐
         │  SHOTLIST ENGINE    │
         └─────────┬──────────┘
                   ↓
         ┌────────────────────┐
         │  PROMPT GENERATOR   │
         └─────────┬──────────┘
                   ↓
    ┌──────────────┴──────────────┐
┌──────────────┐ ┌────────────────┐
│ COMFYUI │ │ VO GENERATOR │
│ (IMAGE/VIDEO) │ │ (TTS) │
└──────┬────────┘ └────────┬───────┘
↓ ↓
└──────────────┬───────────────┘
↓
┌────────────────────┐
│ FFMPEG EDITOR │
└─────────┬──────────┘
↓
┌────────────────────┐
│ FINAL RENDER │
└────────────────────┘

---

## ⚙️ Core Features

### 🎞 Script → Shotlist Engine
- Parses narrative beats
- Converts scenes into structured shot sequences
- Supports cinematic formatting

### 🎯 Prompt Generation System
- Template-driven prompts per shot
- Style locking (lighting, lens, tone)
- Character consistency hooks

### 🧪 Generation Layer
- ComfyUI workflow templates
- Batch rendering support
- Extensible for any diffusion/video model

### 🔊 Voice + Audio
- Plug-in ready for ElevenLabs / TTS providers

### 🎬 Auto-Edit System
- FFmpeg-based timeline assembly
- Caption burn-in
- Rapid preview rendering

---

## 🚀 Quick Start

```bash
git clone https://github.com/YOUR_USERNAME/ai-film-factory.git
cd ai-film-factory

pip install -r requirements.txt
cp .env.example .env

uvicorn app.main:app --reload

http://localhost:8000/docs
    ↓                             ↓

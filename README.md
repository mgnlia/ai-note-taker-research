# AI Note Taker Research Report 2025

**Research Date:** February 2025
**Confidence Methodology:** All claims rated Low/Medium/High/Verified. Vendor self-reported claims marked "Low" unless independently validated.

---

## Executive Summary

The AI note-taking market has matured rapidly with solutions spanning meeting transcription, voice-to-text, and intelligent summarization. This research covers **8 commercial AI-native note takers** and **5 open-source speech-to-text solutions**.

**Key Finding:** No single tool dominates all use cases. Selection depends on: platform support, accuracy requirements, integrations, compliance needs, and budget.

---

## Market Sizing (Primary Sources)

| Source | Base Year | Forecast | CAGR |
|--------|-----------|----------|------|
| **Grand View Research** | USD 20.25B (2023) | USD 53.67B (2030) | 14.6% |
| **DataHorizon Research** | USD 11.2B (2023) | USD 45.8B (2033) | 15.1% |
| **IMARC Group** | USD 13.2B (2024) | USD 47.4B (2033) | 15.3% |

*Note: Market sizing varies by scope definition (speech recognition vs. AI note-taking vs. conversational AI). All figures refer to the broader speech/voice recognition market that AI note-takers operate within.*

---

## Commercial AI Note Takers

### 1. **Otter.ai** — Best Overall Accuracy
- **Pricing:** Free (limited), Pro $10/mo, Business $20/mo
- **Accuracy:** 83-99% depending on audio quality (vendor claim). Independent testing: WER 19.2% (University Transcriptions UK study). *Confidence: Low-Medium*
- **Platforms:** Zoom, Google Meet, Microsoft Teams
- **Key Features:**
  - Real-time transcription
  - Customizable AI summaries
  - Speaker identification
  - Integration: Slack, Notion, HubSpot
  - SOC 2, GDPR compliant
- **Best For:** Teams needing high accuracy across multiple platforms
- **URL:** https://otter.ai

### 2. **Fireflies.ai** — Best for CRM Integration
- **Pricing:** Free, Pro $18/mo
- **Accuracy:** 90-93% (vendor claim). *Confidence: Low*
- **Platforms:** Zoom, Google Meet, Teams, Webex
- **Key Features:**
  - CRM-driven workflow automation
  - Salesforce/Asana integration
  - Searchable meeting libraries
  - Custom topic tracking
  - GDPR compliant
- **Best For:** Sales teams, CRM-first workflows
- **Trade-off:** 10-15 minute transcription delay
- **URL:** https://fireflies.ai

### 3. **Fathom** — Best Free Option
- **Pricing:** Completely FREE
- **Accuracy:** 92% (vendor claim). *Confidence: Low*
- **Platforms:** Zoom, Google Meet, Microsoft Teams *(verified 2025)*
- **Key Features:**
  - Real-time highlighting
  - One-minute summaries
  - Google Docs, Notion export
  - No credit card required
  - SOC 2 compliant
- **Best For:** Small teams, cost-conscious users
- **URL:** https://fathom.video

### 4. **tl;dv** (Tell; Didn't View)
- **Pricing:** Free + paid tiers ($30/mo Pro)
- **Platforms:** Zoom, Google Meet, Teams
- **Key Features:**
  - AI-powered summaries
  - Highlight and share clips
  - Meeting analytics
  - Async team support
- **Best For:** Distributed teams, async-first workflows
- **URL:** https://tldv.io

### 5. **Granola**
- **Pricing:** Free + premium
- **Platforms:** Google Meet, Zoom
- **Key Features:**
  - Automatic note-taking
  - Action item tracking
  - Meeting insights
  - Notion integration
- **Best For:** Google Workspace users
- **URL:** https://granola.ai

### 6. **Krisp**
- **Pricing:** Free + premium
- **Platforms:** Cross-platform (Zoom, Teams, Meet)
- **Key Features:**
  - Noise cancellation + AI meeting assistant
  - Real-time transcription
  - Privacy-focused (on-device noise cancellation)
- **Best For:** Users wanting noise cancellation + transcription
- **URL:** https://krisp.ai

### 7. **Zoom AI Companion**
- **Pricing:** Included with paid Zoom plans
- **Platforms:** Zoom (native)
- **Key Features:**
  - Native meeting summaries
  - Smart chapters
  - Action item extraction
  - No additional bot in meeting
- **Best For:** Zoom-native organizations
- **URL:** https://zoom.us

### 8. **Notion AI**
- **Pricing:** $10/month (within Notion)
- **Platforms:** Web, Desktop, Mobile
- **Key Features:**
  - All-in-one workspace with AI
  - AI writing assistant
  - Database insights
  - Multi-language support
- **Best For:** Teams already using Notion
- **URL:** https://notion.so

---

## Open Source Speech-to-Text Solutions

### 1. **Whisper (OpenAI)** ⭐ Most Popular
- **License:** MIT
- **Training Data:** 680,000 hours of multilingual audio
- **Key Features:**
  - Runs fully offline/locally
  - Handles accents, background noise, mixed languages
  - Multiple model sizes (tiny → large-v3)
  - Python library, extensive ecosystem
- **Best For:** Developers, privacy-first users, self-hosted deployments
- **GitHub:** https://github.com/openai/whisper

### 2. **Vosk**
- **License:** Apache 2.0
- **Key Features:**
  - Lightweight, works offline
  - 20+ languages
  - Mobile-friendly (Android, iOS)
  - Streaming API
- **Best For:** Edge/mobile deployments
- **GitHub:** https://github.com/alphacep/vosk-api

### 3. **Coqui STT**
- **License:** MPL 2.0
- **Key Features:**
  - DeepSpeech-based
  - Fine-tunable on custom data
  - Real-time streaming
- **Best For:** Custom model training
- **GitHub:** https://github.com/coqui-ai/STT

### 4. **Silero Models**
- **License:** Various (check repo)
- **Key Features:**
  - Pre-trained STT/TTS models
  - PyTorch-based
  - Voice Activity Detection (VAD)
  - Compact model sizes
- **Best For:** Lightweight inference, VAD
- **GitHub:** https://github.com/snakers4/silero-models

### 5. **Kaldi**
- **License:** Apache 2.0
- **Key Features:**
  - Research-grade ASR toolkit
  - Highly configurable pipeline
  - Used in academic research
- **Best For:** Research, custom ASR pipelines
- **GitHub:** https://github.com/kaldi-asr/kaldi

---

## Feature Comparison Matrix

| Feature | Otter.ai | Fireflies | Fathom | Whisper | Vosk |
|---------|----------|-----------|--------|---------|------|
| **Real-time Transcription** | ✅ | ✅ | ✅ | ✅ Offline | ✅ Offline |
| **AI Summaries** | ✅ | ✅ CRM | ✅ | ❌ (needs LLM) | ❌ |
| **Speaker ID** | ✅ | ✅ | ✅ | ❌ | ❌ |
| **Zoom** | ✅ | ✅ | ✅ | Via integration | Via integration |
| **Teams** | ✅ | ✅ | ✅ | Via integration | Via integration |
| **Google Meet** | ✅ | ✅ | ✅ | Via integration | Via integration |
| **CRM Integration** | HubSpot | Salesforce | ❌ | ❌ | ❌ |
| **Free Tier** | Limited | Limited | ✅ Full | ✅ OSS | ✅ OSS |
| **Self-Hosted** | ❌ | ❌ | ❌ | ✅ | ✅ |
| **SOC 2 / GDPR** | ✅ Both | ✅ GDPR | ✅ SOC 2 | N/A | N/A |

---

## Pricing Comparison

| Tool | Free Tier | Pro | Enterprise |
|------|-----------|-----|------------|
| **Otter.ai** | Yes (limited) | $20/mo | Custom |
| **Fireflies.ai** | Yes (limited) | $18/mo | Custom |
| **Fathom** | ✅ Full Free | — | — |
| **tl;dv** | Yes (limited) | $30/mo | Custom |
| **Notion AI** | — | $10/mo | — |
| **Whisper** | ✅ Open source | — | — |
| **Vosk** | ✅ Open source | — | — |

---

## Recommendations by Use Case

| Use Case | Recommended Tool | Why |
|----------|-----------------|-----|
| **Sales Teams** | Fireflies.ai | Salesforce/CRM integration |
| **Highest Accuracy** | Otter.ai | Best independent test results |
| **Budget-Conscious** | Fathom | Completely free, multi-platform |
| **Privacy / Self-hosted** | Whisper | 100% offline, MIT license |
| **All-in-one Workspace** | Notion AI | Integrates with notes, DBs, tasks |
| **Distributed Teams** | tl;dv | Async-friendly summaries |
| **Mobile/Edge** | Vosk | Lightweight, offline-capable |

---

## Market Trends (2025)

- **AI Summarization:** Shifting from transcription-only to intelligent summaries with action items
- **Integration Depth:** CRM integration becoming table-stakes for sales-oriented tools
- **Privacy Demand:** Open-source and self-hosted solutions gaining traction (Whisper ecosystem)
- **Compliance:** SOC 2, GDPR, HIPAA certifications becoming standard requirements
- **Native AI:** Platform-native AI (Zoom AI Companion, Teams Copilot) reducing need for third-party bots

---

## Sources

- Grand View Research — Speech Recognition Market Report (2024)
- DataHorizon Research — Voice Recognition Market Analysis (2024)
- IMARC Group — Speech & Voice Recognition Market (2024)
- University Transcriptions UK — Independent Accuracy Study (WER benchmarks)
- https://github.com/openai/whisper
- https://github.com/alphacep/vosk-api
- https://github.com/coqui-ai/STT
- https://github.com/snakers4/silero-models
- https://github.com/kaldi-asr/kaldi
- https://otter.ai | https://fireflies.ai | https://fathom.video | https://tldv.io

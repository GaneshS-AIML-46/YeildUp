# YieldUp – The Digital Krishi Officer

YieldUp is an innovative AI-powered advisory platform built to provide instant, reliable agricultural support for farmers in their native languages. The system integrates advanced speech recognition (ASRSeemless), computer vision (EfficientNet), and Retrieval-Augmented Generation (RAG) using LangChain to enable multimodal, multilingual interaction via voice, text, and images.

---

## Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Architecture Overview](#architecture-overview)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Data Sources](#data-sources)
- [Contributing](#contributing)
- [License](#license)

---

## Features

- Multilingual voice & text support (local Indian languages including Malayalam)
- Farmer queries by speech, text, and image
- Crop and soil disease detection using images with EfficientNet
- Real-time speech-to-text and translation via ASRSeemless
- Retrieval-Augmented Generation (RAG) using LangChain for accurate query answering
- Context-awareness: responses tailored to crop, soil, region, season
- Escalation of complex queries to human agricultural officers
- Continuous improvement with feedback loop

---

## Tech Stack

- **Frontend:** React Native (mobile app), React.js (officer dashboard)
- **Backend:** FastAPI
- **Databases:** PostgreSQL (structured), MongoDB (unstructured)
- **Speech:** SeamlessM4TIndicSeamless (speech-to-text, TTS)
- **Vision:** EfficientNet (crop/soil disease detection)
- **NLP & Retrieval:** Google Gemini, LangChain-powered RAG

---

## Architecture Overview

The farmer interacts through a mobile app with voice, text, or images. ASRSeemless transcribes audio, and EfficientNet processes images for visual diagnosis. A FastAPI backend manages queries, utilizing a RAG pipeline (LangChain) to access structured and unstructured agricultural data. Answers are tailored using regional context, and unresolved queries are escalated to agri-officers. A feedback loop helps refine AI predictions over time.

---

## Setup Instructions

1. **Clone the repository**
2. Install dependencies using the requirements.txt and package.json files.
3. Configure API keys and database URIs in the `.env` file.
4. Train or download ASRSeemless and EfficientNet models.
5. Start backend and frontend servers.
6. Optionally seed database with agricultural data.

---

## Usage

- Farmers ask queries via voice, text, or image on the mobile app.
- Receive automated, regionalized advice, or get routed to an agri-officer if needed.
- Officers use a dashboard to monitor escalations and provide expert responses.

---

## Data Sources

- Indian agricultural knowledge bases
- Real-time regional weather and crop datasets
- Open-source speech and vision datasets for model training

---

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for bug reports, feature requests, or improvements.

---

## License

This project is licensed under the MIT License.


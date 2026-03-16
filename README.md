# LLM Architecture Explorer

An interactive, visual gallery for exploring and comparing the architectures of major Large Language Models (LLMs). Built as a single-page web application with no build step required.

## Features

### 1. Visual Card Gallery
Browse 12 major LLM architectures — GPT-2, GPT-3, GPT-4, BERT, T5, LLaMA, Mistral 7B, Gemini, Claude, PaLM, Phi-2, and Mamba. Each card displays the model name, company, parameter count, release year, architecture family, key innovations, and feature tags.

### 2. Interactive Architecture Diagrams
Click any model card to open a detailed modal with a visual block diagram of its architecture. Diagrams show labeled components (attention heads, FFN layers, normalization layers, position encodings, etc.) rendered as CSS-styled SVG.

### 3. Comparison Mode
Select 2–3 models and compare their architectures side by side. View differences across 11 dimensions: year, parameters, architecture family, layers, attention heads, model dimension, context length, vocabulary, normalization, activation, and position encoding.

### 4. Timeline View
A chronological timeline showing the evolution of LLM architectures from BERT (2018) through the latest 2023–2024 models, highlighting how each model built on prior innovations.

### 5. Filter & Sort
- **Search**: Full-text search across model names, companies, innovations, and tags
- **Sort**: By year (ascending/descending), parameter count, or name
- **Family filter**: All, Decoder-Only, Encoder-Only, Encoder-Decoder, or SSM

### 6. Dark/Light Theme
Toggle between a rich dark theme (blues/teals with glassmorphism) and a clean light theme. Defaults to dark.

## Technical Details

- **Single file**: `index.html` with embedded CSS and JavaScript — no build step
- **No dependencies**: Fully self-contained, no external JavaScript libraries
- **Fonts**: Cabinet Grotesk (display) and Satoshi (body) via Fontshare, JetBrains Mono (monospace) via Google Fonts
- **Responsive**: Mobile-first with a bottom navigation bar on small screens
- **Accessible**: Semantic HTML, keyboard navigation (Escape to close modals), focus rings, ARIA labels

## Models Included

| Model | Company | Year | Params | Family |
|-------|---------|------|--------|--------|
| BERT | Google | 2018 | 340M | Encoder-Only |
| GPT-2 | OpenAI | 2019 | 1.5B | Decoder-Only |
| T5 | Google | 2019 | 11B | Encoder-Decoder |
| GPT-3 | OpenAI | 2020 | 175B | Decoder-Only |
| PaLM | Google | 2022 | 540B | Decoder-Only |
| GPT-4 | OpenAI | 2023 | ~1.8T (MoE) | Decoder-Only |
| LLaMA | Meta | 2023 | 65B | Decoder-Only |
| Mistral 7B | Mistral AI | 2023 | 7.3B | Decoder-Only |
| Gemini | Google DeepMind | 2023 | ~1T+ | Decoder-Only (Multimodal) |
| Claude | Anthropic | 2023 | ~130B (est.) | Decoder-Only |
| Phi-2 | Microsoft | 2023 | 2.7B | Decoder-Only |
| Mamba | Albert Gu & Tri Dao | 2023 | 2.8B | SSM |

## Inspiration

Inspired by [Sebastian Raschka's LLM Architecture Gallery](https://sebastianraschka.com/llm-architecture-gallery/), a viral Hacker News post showcasing visual diagrams of different LLM architectures.

## Usage

Open `index.html` in any modern web browser. No server required.

---

Created with [Perplexity Computer](https://www.perplexity.ai/computer)

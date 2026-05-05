# ✦ Nishith's Paraphraser

A lightweight web-based application for **local text paraphrasing**
using **Ollama**. This project provides an interactive UI to rewrite
text in different tones and styles, with adjustable paraphrasing
strength.

------------------------------------------------------------------------

## 🚀 Features

-   ✍️ Paraphrase text using local LLMs via Ollama\
-   🎨 Multiple writing modes:
    -   Standard
    -   Formal
    -   Casual
    -   Concise
    -   Academic
    -   Creative\
-   🎚 Adjustable rewrite strength (Light, Balanced, Heavy)\
-   ⚡ Fully local execution (no API key required)\
-   🖥 Simple and responsive web interface

------------------------------------------------------------------------

## 🛠 Tech Stack

-   **Frontend:** HTML, CSS, JavaScript\
-   **Backend (local):** Ollama\
-   **Model:** e.g. `llama3.2`, `mistral`, `qwen2.5`

------------------------------------------------------------------------

## 📦 Prerequisites

-   Python 3\
-   Ollama → https://ollama.com

------------------------------------------------------------------------

## ⚙️ Setup & Run

### 1. Install and Start Ollama

``` bash
ollama pull llama3.2
export OLLAMA_ORIGINS="*"
ollama serve
```

Keep this terminal running.

------------------------------------------------------------------------

### 2. Start Local Web Server

``` bash
cd YOUR_PROJECT_FOLDER
python3 -m http.server 5500
```

------------------------------------------------------------------------

### 3. Open the Application

Open in browser:

http://127.0.0.1:5500/index.html

> Do NOT open the HTML file directly (CORS issue)

------------------------------------------------------------------------

## 🧪 Usage

1.  Enter or paste your text\
2.  Select a writing mode\
3.  Adjust rewrite strength\
4.  Click **Paraphrase**\
5.  Copy the result

------------------------------------------------------------------------

## 🔌 API Test (Optional)

``` bash
curl -X POST http://127.0.0.1:11434/api/generate \
-H "Content-Type: application/json" \
-d '{"model":"llama3.2","prompt":"Paraphrase: I am happy today.","stream":false}'
```

------------------------------------------------------------------------

## ⚠️ Notes

-   Ensure Ollama is running\
-   Use a local server (not file://)\
-   Output quality depends on the model

------------------------------------------------------------------------

## 👤 Author

**Nishith Ranjan Biswas**

# 🧠  DryRunBuddy v2.5 Studio

DryRunBuddy is a zero-spoiler, open-source Data Structures & Algorithms (DSA) Socratic Coach. Powered by local, open-weight AI models (Gemma 2 via Ollama), it helps developers build real problem-solving intuition instead of just giving away the solution.

Built for the **Hacktoberfest Weekend Challenge: Build for a Friend**.

## ✨ Features
- **Zero-Spoiler Socratic Coaching:** Analyzes your intuition and gives complexity estimates, counter-examples, and nudges without revealing the exact code.
- **Code Debugger:** Identifies exact line-by-line bugs in your attempt and provides patched snippets.
- **100% Local & Private:** Runs entirely on your machine using Ollama and Gemma 2. No cloud APIs, no data collection.
- **Markdown Export:** Generates beautiful, structured study notes (.md) for Notion or Obsidian.
- **Built-in DSA Studio:** Comes with 10 curated classic DSA patterns (Sliding Window, Binary Search, Graphs, DP, Stack, Hashing, etc.) packed with intentional bugs for you to practice.
- **Custom Problem Support:** Paste any LeetCode problem statement to get real-time Socratic coaching on it.
- **Quick Revision Notes:** Context-aware data structure cheat-sheets appear for every problem to help you remember the optimal patterns.

## 🚀 Getting Started

### 1. Install Ollama
Download and install [Ollama](https://ollama.com/).

### 2. Pull the Gemma Model
```bash
ollama pull gemma2:2b
```

### 3. Start the Local Server with CORS
DryRunBuddy needs to communicate with Ollama directly from your browser. Start Ollama with:
**Windows (PowerShell):**
```powershell
$env:OLLAMA_ORIGINS="*"
ollama serve
```
**Mac/Linux:**
```bash
OLLAMA_ORIGINS="*" ollama serve
```

### 4. Open the App
Simply open `index.html` in your web browser, or view the live demo (if using the instant offline engine).

## 🛠️ Built With
- **Vanilla HTML/JS/CSS** + TailwindCSS via CDN
- **Ollama** (Local Inference)
- **Gemma 2 (2B)** (Open-Weight Model by Google)

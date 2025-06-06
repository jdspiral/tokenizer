# Tokenizer

**See how language models fragment, encode, and simulate meaning.**

Tokenizer is an interactive demo that lets you explore what your sentence looks like to a machine — from tokenization to embeddings, grammar trees, and beyond.

---

## What It Does

- Enter any sentence (default: *"The young student didn't submit the final report on time."*)
- See how models **tokenize** and **encode** your words
- Explore **POS tagging** and **dependency parsing**
- Visualize **BERT embeddings** in 2D
- Extract **Subject–Verb–Object (SVO)** triples from your text
- Learn how machines simulate understanding through structure, not grounding

## How This Relates to LLMs

This app combines classical NLP visualizations (e.g., POS tagging, dependency parsing) with real language model embeddings (from DistilBERT) to help users "see" how structure and meaning are derived.

**But! Important clarification:**

- ✅ **Tokenization** and **embeddings** represent real components of LLM internals.
- ⚠️ **Dependency trees, POS tags, and SVOs** are illustrative—they reflect *our* grammatical intuition, not how models “think.”

To understand actual LLM internals:
- [What BERT Knows About Syntax](https://arxiv.org/abs/1906.04341)
- [Transformer Circuits](https://transformer-circuits.pub)
- [Is POS Even Real?](https://arxiv.org/abs/2005.04511)

---

## Why It Matters
LLMs don’t “understand” language like humans do. They simulate meaning through statistical patterns, not embodied experience.

- They don’t know what a dog feels like.

- But they know what often comes after “pet the…”

**Tokenizer** lets you see how this works — and why it matters in an era where AI writes resumes, moderates speech, and shapes how truth circulates.

---

## How It Works

Built with:
- **Streamlit** for UI
- **spaCy** for grammar & dependency parsing
- **HuggingFace Transformers** for tokenization and BERT embeddings
- **Plotly** + **PCA** for interactive visualization

---

## 🚀 Live Demo

Try it here → [Launch Tokenizer](https://meaning-machine.streamlit.app/)

---

## Run It Locally

```bash
git clone https://github.com/yourusername/tokenizer.git
cd tokenizer
python -m venv venv
source venv/bin/activate        # or .\venv\Scripts\activate on Windows
pip install -r requirements.txt
python -m spacy download en_core_web_sm
streamlit run app.py
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

---

Built by [Josh Hathcock](https://theperformanceage.com/)

Thinking out loud in code.
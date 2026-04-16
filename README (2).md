# Text Summarizer

An NLP-based text summarization tool that runs **entirely in the browser** — no API, no internet connection, no back-end, and no cost.

## How It Works

Uses **extractive summarization**: a classic NLP technique that scores each sentence in the text based on word frequency, then selects the top-ranked sentences to form the summary. The original sentences are preserved in order so the summary reads naturally.

**Algorithm steps:**
1. Split text into individual sentences
2. Build a word-frequency map (ignoring common stop words)
3. Score each sentence by the average frequency of its words
4. Apply position-based boosting (first/last sentences get a bonus for "general" focus)
5. Pick the top N sentences and restore their original order

## Features

- 5 summary length options (1 to 7 sentences)
- 3 focus modes: General, Opening ideas, Keyword-rich
- Live word count
- Compression stats (original words, summary words, % reduction)
- Copy to clipboard
- Download as `.txt`
- Works offline — no API or internet required

## Tech Stack

- HTML5, CSS3, Vanilla JavaScript
- Zero dependencies, zero API calls

## How to Use

1. Clone or download this repo
2. Open `index.html` in any browser
3. Paste your text, choose options, click **Summarize**

## Deploy to GitHub Pages

1. Push to GitHub
2. Go to **Settings → Pages → Source: main branch**
3. Share your live link!

## Project Structure

```
text-summarizer/
├── index.html
└── README.md
```

## License

MIT

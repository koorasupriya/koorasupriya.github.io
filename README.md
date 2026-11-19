# koorasupriya.github.io

Personal portfolio of **Supriya Koora**, GenAI & Data Engineer.

Live at **https://koorasupriya.github.io**

- A single static page (`index.html`): hand-written HTML, CSS and vanilla JS, no build step and no dependencies apart from Google Fonts.
- **Career trace**: work history drawn as an OpenTelemetry-style span waterfall. Click a span to see its attributes.
- **Ask my portfolio**: a small in-browser RAG system. BM25 retrieval over 25 passages, streamed answers with numbered citations, and a per-answer trace. No LLM, no network calls.
- Light and dark themes, keyboard accessible, respects `prefers-reduced-motion`.

## Run locally

```bash
python -m http.server 8080
# open http://localhost:8080
```

## Update content

Everything is in `index.html`:

| What | Where |
| --- | --- |
| Career trace spans | `const spans = [...]` |
| Repo explorer | `const repos = [...]` |
| "Ask my portfolio" knowledge | `const KB = [...]` (one passage per fact; `k` holds extra search keywords) |
| Experience, skills, credentials | Static HTML sections |

# MatterPlay

MatterPlay is an interactive science playground that turns learning physics into hands-on experiments. Learners can explore forces, energy, and circuits, change variables, observe what happens, and ask the built-in Science Tutor questions about the science behind their experiments.

## Features

- **Force Lab** — explore forces and motion through interactive activities.
- **Energy Lab** — investigate energy and how it changes during an activity.
- **Circuit Lab** — explore basic electrical circuit concepts.
- **Science Tutor** — ask questions in natural language and receive experiment-aware explanations powered by Google Gemini through a Cloudflare Worker.
- **Responsive, single-page experience** — the main application is delivered as one HTML file.

## Run locally

1. Download or clone this repository.
2. Open `index.html` in a modern web browser.
3. An internet connection is needed for the AI Science Tutor and externally hosted fonts. The interactive labs themselves are part of the HTML application.

## AI architecture

The browser sends the learner's question and current experiment context to a Cloudflare Worker. The Worker calls the Google Gemini API and returns the tutor's response.

The Gemini API key is intended to be stored as a Cloudflare Worker secret (`GEMINI_API_KEY`). **Do not put the Gemini API key in this repository or in `index.html`.**

## Technologies

- HTML, CSS, and JavaScript
- Cloudflare Workers
- Google Gemini API

## Project status

Built as a web-based educational science playground for the IceHacks 2026 hackathon.

## Credits and AI disclosure

MatterPlay is an independently developed project. Generative AI tools were used as development assistance, including for coding and the AI-powered Science Tutor. The tutor uses the Google Gemini API through a Cloudflare Worker.

---

For the live application and project demonstration, see the links added to this repository's project description and the hackathon submission.

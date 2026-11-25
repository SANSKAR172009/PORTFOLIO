# Sanskar Soni Portfolio

Personal portfolio for [sanskarsoni.vercel.app](https://sanskarsoni.vercel.app/). The site is a static, single-page application built with HTML, CSS, and JavaScript. The page source is in `index.html`; the profile image is in `assets/`.

## Technical Projects

### NEBULA — Groq AI Playground

- **Problem:** Model experiments are harder to inspect when prompt controls, model selection, and request feedback are spread across separate tools.
- **Solution and architecture:** A JavaScript browser interface connects to a Groq API client for model requests and streamed responses. The repository also documents an optional Vercel Edge API route for proxy deployment. The streaming-style preview on this portfolio is simulated; it is not a live benchmark.
- **Technology:** JavaScript, HTML, CSS, Groq API, `ReadableStream`/SSE, Vercel.
- **My contribution:** Built the playground UI, model and prompt controls, stream display, and inference telemetry.
- **Code and documentation:** [GROQ-PLAYGROUND repository and README](https://github.com/SANSKAR172009/GROQ-PLAYGROUND).

### MiniGit — Python Version-Control CLI

- **Problem:** Familiar Git commands hide how file contents become objects, trees, staged entries, and commits.
- **Solution and architecture:** A Python CLI separates command handlers from shared repository helpers. The helpers manage SHA-1-addressed objects, trees and commits, the staging index, references, and working-tree paths.
- **Technology:** Python, SHA-1, zlib, CLI.
- **My contribution:** Built the Python implementation and the interactive command walkthrough in this portfolio. The browser walkthrough prints a demonstration; it does not execute the Python CLI.
- **Code and documentation:** [MiniGit source](https://github.com/SANSKAR172009/LLM-PIPELINE-EXPLORER/tree/main/src/minigit), [architecture guide](https://github.com/SANSKAR172009/LLM-PIPELINE-EXPLORER/blob/main/docs/ARCHITECTURE.md), and [internals walkthrough](https://github.com/SANSKAR172009/LLM-PIPELINE-EXPLORER/blob/main/docs/internals-walkthrough.md).

<a id="interactive-attention-demo"></a>

### Self-Attention Explorer

- **Problem:** Attention relationships can be difficult to discuss without a visual example.
- **Solution and architecture:** A browser UI lets a visitor select one of four words and updates score bars from a fixed example-weight map. The weights are illustrative; the demo does not run a transformer or produce model outputs.
- **Technology:** JavaScript, HTML, CSS, DOM events.
- **My contribution:** Implemented the token interaction, score-bar rendering, and explanation of the demo's scope.
- **Code and documentation:** [Portfolio source](https://github.com/SANSKAR172009/PORTFOLIO/blob/main/index.html).

## S&AI-Projects Contributions

All ten pull requests below were submitted to [S-AI-Projects/ML-For-Beginners](https://github.com/S-AI-Projects/ML-For-Beginners) between 18 and 20 November 2026. Their status was open on 25 November 2026.

| Task ID | Contribution | Pull request |
| --- | --- | --- |
| R37-T011 | Bounded reinforcement-learning state-chain example | [#77](https://github.com/S-AI-Projects/ML-For-Beginners/pull/77) |
| R37-T012 | Cosine similarity boundary example | [#78](https://github.com/S-AI-Projects/ML-For-Beginners/pull/78) |
| R37-T013 | Scenario rubric checker | [#92](https://github.com/S-AI-Projects/ML-For-Beginners/pull/92) |
| R37-T014 | Local token-budget preflight | [#93](https://github.com/S-AI-Projects/ML-For-Beginners/pull/93) |
| R37-T015 | Offline token-budget adapter | [#94](https://github.com/S-AI-Projects/ML-For-Beginners/pull/94) |
| R37-T016 | Introduction lesson rubric example | [#95](https://github.com/S-AI-Projects/ML-For-Beginners/pull/95) |
| R37-T017 | Chronological time-series split | [#96](https://github.com/S-AI-Projects/ML-For-Beginners/pull/96) |
| R37-T018 | Validate tool actions before execution | [#97](https://github.com/S-AI-Projects/ML-For-Beginners/pull/97) |
| R37-T019 | Real-world scenario rubric exercise | [#98](https://github.com/S-AI-Projects/ML-For-Beginners/pull/98) |
| R37-T020 | Binary classification metrics lab | [#99](https://github.com/S-AI-Projects/ML-For-Beginners/pull/99) |

## Run Locally

This is a static site with no package installation step. From the repository directory, run:

```sh
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

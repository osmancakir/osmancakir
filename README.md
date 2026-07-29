## Osman Cakir

AI engineer in Munich. I build multi-agent systems and the products around them, which
means I also write the frontend, the schema, the tests and the deploy pipeline. Most of my
work sits where language models meet real collections: news, books, museum archives,
research metadata.

Before software I studied economics and art history. That is why my agents tend to be
evaluated rather than demoed.

### Selected work

**[libraryuniverse-news-desk](https://github.com/osmancakir/libraryuniverse-news-desk)** ·
LangGraph, TypeScript, OpenAI

A multi-agent newsroom that runs in production. Five journalist personas research the day's
stories in parallel and pitch; a human editor selects; the pipeline then writes each story
at three CEFR levels of German, repairs its own schema and encoding errors through a
validator agent, illustrates it, narrates it into three audio tracks, and publishes to a
CMS. Parallel fan-out with state reducers, two human-in-the-loop interrupts, structured
output captured through Zod-typed tools.

**[Library Universe](https://libraryuniverse.com)** · React Router, TypeScript, Postgres, Sanity, fly.io

The platform the news desk feeds: news for German learners, with graded reading levels,
vocabulary flashcards on a spaced-repetition schedule, audio, and a book catalogue.
249 commits, 225 TypeScript modules, Vitest and Playwright suites, GitHub Actions deploy.
Source is private; the [reading
extension](https://github.com/osmancakir/libraryuniverse-reading-extension) that pairs with
it is not.

**Städel Museum** · multimodal LLM evaluation *(freelance, 2026)*

An AI metadata pipeline for artwork collections built on several multimodal models, with an
evaluation workflow behind it: weighted scoring categories, blind comparison of model
responses, and bias control conditions, plus a research interface for curators to review
the output. The point was to find out which model an art-historical institution should
actually trust, not to assume one.

**[candidgarden.com](https://candidgarden.com)** · vector search, human-AI verification *(LMU Munich, with Prof. Dr. Kohle)*

54,000 artworks processed in three languages through hybrid human-AI verification
protocols, producing iconographic metadata broader than the source catalogues carried.
On top of it, a semantic search interface over vector embeddings with a query-decomposition
agent, so a conceptual question finds work that shares no keyword with it.
Coding Da Vinci Süd award for the technically most demanding project.

**[agent-skills](https://github.com/osmancakir/agent-skills)** · Agent Skills for Claude Code and Codex

Installable skills, each with its own resources: a Bavarian public-sector job search that
maintains a deduplicated database and scores ads against a candidate profile, and a cue-card
generator that turns speaker notes into a printable duplex PDF deck.

**[DataCite Metadata Generator](https://github.com/osmancakir/rdm_datacite_new)** · React, TypeScript

Research data management tooling for DataCite metadata and XML generation, built for LMU
University Library and [in
use](https://dhvlab.gwi.uni-muenchen.de/datacite-generator/) there. Three generations, from
a single-file jQuery tool to a
[React rewrite](https://rdm-datacite-new.fly.dev/).

### What I work with

- **AI** LangChain, LangGraph, RAG, pgvector, model evaluation, prompt and output-schema design, Claude Code, Codex
- **Frontend** React, React Router, TypeScript, TanStack Query, Tailwind, Radix UI, Next.js, TensorFlow.js
- **Backend** Node.js, Postgres, SQLite and LiteFS, Python, Sanity, AWS S3 and RDS
- **Ops** Docker, fly.io, AWS EC2 and CloudFront, GitHub Actions, Linux
- **Testing** Vitest, Playwright, MSW, Sentry

### Also

Five years of enterprise access-management dashboards at evolutionID GmbH, including a
biometric photo capture module made roughly 50x faster by moving face detection into the
browser with TensorFlow.js. DAAD scholarship, MSc Economics at LMU Munich.

Reachable at osmancakir11@gmail.com.

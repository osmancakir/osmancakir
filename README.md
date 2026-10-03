## Osman Cakir

AI engineer in Munich. I build multi-agent systems and the products around them, which
means I also write the frontend, the schema, the tests and the deploy pipeline. Most of my
work sits where language models meet real collections: news, books, museum archives,
research metadata.

Before software I studied economics and art history. That is why my agents tend to be
evaluated rather than demoed.

### Selected work

**[umbruchai-news-desk](https://github.com/osmancakir/umbruchai-news-desk)** ·
LangGraph, TypeScript, OpenAI

A multi-agent newsroom that runs in production, and the backend of
[umbruchai.com](https://umbruchai.com). Five journalist personas research the day's stories
in parallel and pitch; a human editor selects; the pipeline then writes each story at three
CEFR levels of German, repairs its own schema and encoding errors through a validator
agent, illustrates it, narrates it into three audio tracks, and publishes to a CMS.
Parallel fan-out with state reducers, two human-in-the-loop interrupts, structured output
captured through Zod-typed tools. Open source, including all seven agent definitions.

**[umbruchai](https://github.com/osmancakir/umbruchai)** · React Router 7, Cloudflare Workers, Sanity

The publication the news desk writes into: [umbruchai.com](https://umbruchai.com), a German
AI-journalism site now carrying 87 pieces across seven sections, each readable at three
CEFR levels with audio at every level, and a page per agent author. Also open source, so
the newsroom and the paper it prints can be read end to end.

**[candidgarden_web](https://github.com/osmancakir/candidgarden_web)** · React Router 7, pgvector, three.js, Cloudflare Workers *(LMU Munich, with Prof. Dr. Kohle)*

An institute for art re-search, now open source. Deployed at
[candidgarden.com](https://candidgarden.com), it holds 54,497 artworks from the ARTigo
corpus, processed in three languages through hybrid human-AI verification, each read at
Erwin Panofsky's three levels of meaning. The readings stay labelled provisional and
confidence reports observed agreement rather than truth.
Search embeds the query with `bge-m3` and ranks it against 1,024-dimensional vectors in
Postgres with pgvector, so a conceptual question finds work that shares no keyword with it.

The [Atlas](https://candidgarden.com/archive/atlas) puts 89,800 of those readings into one
WebGL point cloud. Its UMAP layout is fitted offline and never moves, so a search lights up
matches inside a fixed space instead of rearranging it, and two searches stay comparable; a
custom binary format ships the geometry in 1.6 MB rather than 8 MB of JSON. Server-rendered
on Cloudflare Workers over Hyperdrive to a private RDS, with Vitest, Playwright and both
runtimes built in CI.

**[ai-political-leanings](https://github.com/osmancakir/ai-political-leanings)** · LLM evaluation, Python

Six frontier models answered the Political Compass's 59 propositions in English, German and
Turkish: 1,062 answers, no refusals, no missing cells, scored on both axes. Five of six sit
left-libertarian in every language, and the prompt language moves the result
systematically, with German producing the most libertarian score for all six models.

**[Library Universe](https://libraryuniverse.com)** · React Router, TypeScript, Postgres, Sanity, fly.io

A library for reading and learning: a book catalogue and vocabulary flashcards on a
spaced-repetition schedule. The [reading
extension](https://github.com/osmancakir/libraryuniverse-reading-extension) that pairs with
it is here.

**Städel Museum** · multimodal LLM evaluation *(freelance, 2026)*

An AI metadata pipeline for artwork collections built on several multimodal models, with an
evaluation workflow behind it: weighted scoring categories, blind comparison of model
responses, and bias control conditions, plus a research interface for curators to review
the output. The point was to find out which model an art-historical institution should
actually trust, not to assume one.


**[DataCite Metadata Generator](https://github.com/osmancakir/rdm_datacite_new)** · React Router, TypeScript

A guided form that turns DataCite's deeply conditional kernel-4 schema into valid XML, with
round-trip editing of records that already exist. Constraint-aware validation, so the
repository stops rejecting submissions for reasons nobody can see.
[Live](https://rdm-datacite-new.fly.dev/).

This is my own rebuild of a problem I worked on at LMU Munich, where I contributed 12
commits to the University Library's
[DataCite generator](https://github.com/UB-LMU/datacite-metadata-generator), which is
[in production](https://dhvlab.gwi.uni-muenchen.de/datacite-generator/) at the UB.

### What I work with

- **AI** LangChain, LangGraph, RAG, pgvector, embeddings and UMAP projection, model evaluation, prompt and output-schema design, Claude Code, Codex
- **Frontend** React, React Router, TypeScript, TanStack Query, Tailwind, Radix UI, Next.js, three.js and WebGL, TensorFlow.js
- **Backend** Node.js, Postgres, SQLite and LiteFS, Python, Sanity, AWS S3 and RDS
- **Ops** Docker, fly.io, Cloudflare Workers, AWS EC2 and CloudFront, GitHub Actions, Linux
- **Testing** Vitest, Playwright, MSW, Sentry

### Also

Five years of enterprise access-management dashboards at evolutionID GmbH, including a
biometric photo capture module made roughly 50x faster by moving face detection into the
browser with TensorFlow.js. DAAD scholarship, MSc Economics at LMU Munich.

Reachable at osmancakir11@gmail.com.

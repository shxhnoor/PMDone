# PMDone

**An LLM-powered symptom navigator built with the Anthropic API.**

PMDone helps users make sense of how they're feeling before deciding what to do next — whether that's rest, a pharmacy visit, or booking a doctor. Instead of a search engine returning a wall of possibilities, PMDone routes you based on your current state and lets Claude reason through your symptoms conversationally.

> 🚧 **Active development** — core routing and UI are functional; backend integrations and full conversation flow are in progress.

---

## What it does

- Presents five mood-based entry points so users can describe how they feel in plain language
- Routes each entry to a dedicated page with a tailored Claude-powered conversation
- Uses the Anthropic API as the reasoning layer — not just for text generation, but to guide what questions to ask and what to suggest next
- Stores session data via Supabase/PostgreSQL for continuity

---

## Tech stack

| Layer | Tool |
|---|---|
| Framework | Next.js (App Router) |
| Language | TypeScript |
| Styling | Tailwind CSS |
| AI | Anthropic API (Claude) |
| Database | Supabase / PostgreSQL |
| Deployment | Vercel |

---

## Project structure

```
/app
  /page.tsx           → Homepage with mood-based routing
  /[mood]/page.tsx    → Five symptom entry routes
/components           → Shared UI components
/lib                  → Anthropic API client + Supabase config
```

---

## Why I built this

I wanted to explore what it actually looks like to use Claude as infrastructure rather than a chatbot — where the model is doing real reasoning work inside a product, not just answering questions. Healthcare navigation felt like a good test case: the stakes are real, the information is messy, and getting the routing right matters.

It's also a personal interest area. I study CS and Statistics at Queen's and have a background in pharmacology-adjacent research, so health tech is somewhere I want to spend more time.

---

## Status

- [x] Homepage + five mood routing pages
- [x] Dark lunar ocean UI theme
- [x] Anthropic API integration (Claude as reasoning layer)
- [x] Basic Supabase setup
- [ ] Full multi-turn conversation flow
- [ ] Symptom history + session persistence
- [ ] Mobile polish + accessibility pass

---

## Contact

Shahnoor — [your email] · [LinkedIn if you want]

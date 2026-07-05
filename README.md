# pm-interview.md

Battle-tested prompts for practicing Product Manager interview questions with any LLM. Paste one as a system prompt and the model becomes a brutally honest interview coach that walks you through your answer one section at a time.

Two prompts to start:

| Prompt | What it drills | Open in Claude | Open in ChatGPT | Raw |
| --- | --- | :---: | :---: | :---: |
| **Favorite Product** | Product taste, customer empathy, business/strategy, improvement + metrics | [![Open in Claude](https://img.shields.io/badge/Open_in_Claude-000?logo=anthropic&logoColor=white)](https://claude.ai/new?q=Act%20as%20a%20PM%20interview%20coach.%20Fetch%20and%20follow%20this%20system%20prompt%20verbatim%3A%20https%3A%2F%2Fraw.githubusercontent.com%2Fsendishani%2Fpm-interview.md%2Fmain%2Fprompts%2Ffavorite-product.md) | [![Open in ChatGPT](https://img.shields.io/badge/Open_in_ChatGPT-10a37f?logo=openai&logoColor=white)](https://chatgpt.com/?prompt=Act%20as%20a%20PM%20interview%20coach.%20Fetch%20and%20follow%20this%20system%20prompt%20verbatim%3A%20https%3A%2F%2Fraw.githubusercontent.com%2Fsendishani%2Fpm-interview.md%2Fmain%2Fprompts%2Ffavorite-product.md) | [`.md`](prompts/favorite-product.md) |
| **Root Cause Analysis** | Structured diagnosis of metric drops — clarify, segment, hypothesize, prioritize, fix | [![Open in Claude](https://img.shields.io/badge/Open_in_Claude-000?logo=anthropic&logoColor=white)](https://claude.ai/new?q=Act%20as%20a%20PM%20interview%20coach.%20Fetch%20and%20follow%20this%20system%20prompt%20verbatim%3A%20https%3A%2F%2Fraw.githubusercontent.com%2Fsendishani%2Fpm-interview.md%2Fmain%2Fprompts%2Froot-cause-analysis.md) | [![Open in ChatGPT](https://img.shields.io/badge/Open_in_ChatGPT-10a37f?logo=openai&logoColor=white)](https://chatgpt.com/?prompt=Act%20as%20a%20PM%20interview%20coach.%20Fetch%20and%20follow%20this%20system%20prompt%20verbatim%3A%20https%3A%2F%2Fraw.githubusercontent.com%2Fsendishani%2Fpm-interview.md%2Fmain%2Fprompts%2Froot-cause-analysis.md) | [`.md`](prompts/root-cause-analysis.md) |

Every prompt is one self-contained markdown file. Paste it as the system prompt and start talking to the model. That's the whole thing.

---

## How to use

### Option 1: One-click (recommended)

Click **Open in Claude** or **Open in ChatGPT** above. The link pre-fills a message asking the model to fetch this repo's raw prompt file and follow it as its system prompt. Say hi and start practicing.

*Note: Claude's web fetch is generally reliable. ChatGPT's browsing depends on your plan; if the fetch fails, fall back to Option 2.*

### Option 2: Copy-paste

1. Open the raw prompt file (e.g. [favorite-product.md](prompts/favorite-product.md)).
2. Select all → copy.
3. Paste it as the **first message** in a new ChatGPT / Claude / other LLM chat.
4. Send. The model will greet you and start coaching.

### Option 3: As a real system prompt

If your LLM UI has a dedicated system-prompt / custom-instructions field (Claude Projects, ChatGPT Custom GPTs, most API playgrounds), paste the file there instead of as a chat message. The behavior is identical, just cleaner.

---

## What "good" looks like

These prompts are opinionated. They will:

- **Refuse to write the answer for you.** Coaching is iterative — you draft, the model critiques.
- **Be brutally honest.** If your segmentation is lazy, they will say so. No cushioning.
- **Walk the framework one section at a time.** No 3000-word dumps.
- **Steelman before attacking.** Your argument gets rebuilt to its strongest form first.
- **Show gold examples on request.** "Too Good To Go," "Flighty" (Favorite Product), "TikTok LIVE" (RCA) — offered as illustrations, not dumped unprompted.

If you want a chatbot that tells you your answer is great, use a different one.

---

## Repo layout

```
pm-interview.md/
├── prompts/         # paste-ready system prompts (works with any LLM)
├── examples/        # annotated gold transcripts (coming soon)
├── CHANGELOG.md
└── LICENSE
```

---

## Contributing

New prompts, better framework sections, or annotated gold transcripts are all welcome. Open a PR with:

- A specific interview question type (e.g. estimation, product design, execution)
- A single self-contained `.md` file in `prompts/` structured as: **role → behavior rules → first turn → reference framework**
- One example session showing what a good coaching turn looks like

Keep the "no-yapping, brutally honest, one-section-at-a-time" tone. That's the point of view of this repo.

---

## License

MIT. Use these prompts anywhere — training, teaching, your own coaching product, resale, whatever. Attribution appreciated but not required.

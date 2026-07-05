# pm-interview.md

**System prompts to practice Product Manager interviews with ChatGPT, Claude, or any agent.** Free, MIT-licensed, and structured as opinionated coaching flows — paste one file into the model and it walks you through drafting a strong answer to a Favorite Product or Root Cause Analysis (RCA) interview question, one section at a time, with brutally honest feedback.

Built for APM / PM candidates preparing for interviews at Google, Meta, Amazon, Uber, Stripe, TikTok, and any other company that runs product-sense or metric-diagnosis rounds.

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
3. Paste it as the **first message** in a new ChatGPT / Claude / other agent chat.
4. Send. The model will greet you and start coaching.

### Option 3: As a real system prompt

If your agent UI has a dedicated system-prompt / custom-instructions field (Claude Projects, ChatGPT Custom GPTs, most API playgrounds), paste the file there instead of as a chat message. The behavior is identical, just cleaner.

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
├── prompts/         # paste-ready system prompts (works with any agent)
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

## FAQ

### What's the best ChatGPT / Claude prompt for practicing PM interviews?
The two files in this repo (`prompts/favorite-product.md` and `prompts/root-cause-analysis.md`) are structured as full system prompts specifically for coaching, not for generating cookie-cutter answers. They critique your drafts one section at a time instead of writing the whole answer for you — which is what makes them work as practice tools.

### How do I use ChatGPT to prepare for a product manager interview?
Open a new chat, paste one of the prompt files as your first message (or into ChatGPT's custom-instructions field), and start drafting. The model will greet you, ask which product / scenario you want to work on, and walk you through the framework step by step. Same pattern in Claude, Gemini, or any other capable agent.

### What is a Favorite Product PM interview question?
A product-sense question asking you to pick a product you love, explain why it's great, identify user segments and pain points, propose an improvement, weigh tradeoffs, and define success metrics. Common at Google APM, Meta RPM, Uber, Stripe, and most consumer / marketplace PM loops. The framework in [`prompts/favorite-product.md`](prompts/favorite-product.md) covers all 14 sections a strong answer needs.

### What is a Root Cause Analysis (RCA) PM interview question?
A metric-diagnosis question like "spend is down 20%, what happened?" or "TikTok LIVE sessions dropped — investigate." Tests structured thinking under ambiguity: clarify the metric, validate instrumentation, segment, build a hypothesis tree, prioritize, name a leading hypothesis, propose fixes, define success. Common at TikTok, Meta, Amazon, DoorDash, Netflix. The framework in [`prompts/root-cause-analysis.md`](prompts/root-cause-analysis.md) walks the full flow.

### Why not just ask ChatGPT directly?
Because default agent behavior is to write a polished answer *for* you — which teaches you nothing. These prompts flip the dynamic: the model refuses to draft the answer, asks *you* to draft, then critiques. That's the difference between reading an interview book and actually rehearsing.

### Does this work for APM programs (Google APM, Meta RPM, Microsoft PM Explore, etc.)?
Yes. The frameworks are calibrated to the senior-PM answer bar used across FAANG + APM programs. If you're targeting a specific company (e.g. TikTok governance, Uber marketplace, Stripe payments), tell the coach at the start of the session and it will tailor the practice scenario.

### Can I use these prompts commercially?
Yes — MIT license. Use them in your own coaching product, in training material, in courses, in a competitor to this repo, whatever. Attribution appreciated but not required.

---

## License

MIT. Use these prompts anywhere — training, teaching, your own coaching product, resale, whatever. Attribution appreciated but not required.

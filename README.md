# pm-interview.md

Battle-tested prompts for practicing Product Manager interview questions with any LLM. No account, no site, no signup — just the prompts.

Two prompts to start:

| Prompt | What it drills | Where |
| --- | --- | --- |
| **Favorite Product** | Product taste, customer empathy, business/strategy, improvement + metrics | [`prompts/favorite-product.md`](prompts/favorite-product.md) |
| **Root Cause Analysis** | Structured diagnosis of metric drops — clarify, segment, hypothesize, prioritize, fix | [`prompts/root-cause-analysis.md`](prompts/root-cause-analysis.md) |

Every prompt is one self-contained markdown file. Paste it as the system prompt, then just start talking to the model. That's the whole thing.

---

## How to use

### Claude (claude.ai, API, or Claude Code)

1. Copy the contents of the prompt file.
2. Paste it as the **system prompt** in a new conversation.
3. Start with something like `Coach me through the favorite product question. My product is Notion.`

### ChatGPT / other chat UIs without a system prompt field

Paste the prompt as your **first message**, followed by:

```
Take on the role described above. My first answer is coming next.
```

Then send your actual practice answer as the second message.

### As a Claude Skill

Each prompt is also packaged as a `.skill` bundle in [`skills/`](skills/). Drop it into your Claude Skills directory and Claude will auto-load it when you ask about that interview type. See the [Anthropic docs](https://docs.anthropic.com) for skill install paths.

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
├── skills/          # Claude Skills bundles (.skill)
├── examples/        # annotated gold transcripts (coming soon)
├── CHANGELOG.md
└── LICENSE
```

---

## Contributing

New prompts, better framework sections, or annotated gold transcripts are all welcome. Open a PR with:

- A specific interview question type (e.g. estimation, product design, execution)
- A single self-contained `.md` file in `prompts/`
- One example session showing what a good coaching turn looks like

Keep the "no-yapping, brutally honest, one-section-at-a-time" tone. That's the point of view of this repo.

---

## License

MIT. Use these prompts anywhere — training, teaching, your own coaching product, resale, whatever. Attribution appreciated but not required.

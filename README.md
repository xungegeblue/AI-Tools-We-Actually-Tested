# AI Tools We Actually Tested

**A short, opinionated list of AI tools — one per job, every one opened and run before it got listed.**

No infinite scroll. No affiliate links. No "top 100 AI tools of the year" padding.

> 中文版：[README.zh-CN.md](README.zh-CN.md)

---

## Why this list is short

There are tens of thousands of AI tools. Almost none of them survive being used twice.

So this repo keeps a deliberately small catalogue: **one strong tool per job**. If a tool here has a flaw worth knowing, the flaw is written down instead of hidden. If a tool is ours, the page says so before you click.

This is the open-source mirror of [MusePics Directory](https://musepics.com/) — same entries, same rules, readable without JavaScript and forkable as plain Markdown.

**Currently listing: 4 tools across 4 categories.**

---

## The list at a glance

| Tool | The job it does | Free tier | Paid |
|---|---|---|---|
| [AIGenerate](https://musepics.com/site/aigenerate) | AI images that keep the same face | 3 images/day, **no signup** | Credits unlock 2K / 4K |
| [Jev FastEval](https://musepics.com/site/jev-fasteval) | Scores text in ~0.3s instead of chatting about it | 10 runs/day (registered) | Pro: 100 runs/day |
| [Musebrain](https://musepics.com/site/musebrain) | Private AI over your own notes and PDFs | Guide free, workspace has free tier | — |
| [LessonCraft](https://musepics.com/site/teacher-ai) | Lesson plans, quizzes and feedback for teachers | Free monthly cap, no card | $12/mo · $84/yr |

---

## Free tier cheat sheet

If you only read one table, read this one — what you get for $0, before paying anything.

| | Free allowance | Signup needed? | What free gets you |
|---|---|---|---|
| **AIGenerate** | 3 images / day | No | Fast tier output, any aspect ratio |
| **Jev FastEval** | 10 runs / day | Yes (no card) | All ten evaluators |
| **Musebrain** | Guide + comparison tables free | No | The methodology; workspace has its own free tier |
| **LessonCraft** | Free monthly cap | Yes (no card) | All three tools, exports included |

---

## AIGenerate — AI image generator with face consistency

`Image generation` · [aigenerate.musepics.com](https://aigenerate.musepics.com)

Most image generators are built for one nice picture. AIGenerate is built for the *second* picture: upload up to 14 reference photos and the face, freckles and eye colour survive a change of outfit, location and lighting.

**What it does well**
- Identity holds across scenes — up to 14 reference photos, and more references hold better when the camera angle changes
- Three quality tiers with the credit cost shown *before* you click generate: Fast, Standard (2K), Identity (4K)
- Plain English or Chinese gets rewritten into a structured English prompt before it reaches the model — no prompt engineering required
- Text-to-image, image-to-image, a character mode, and a public Explore gallery
- Aspect ratios: 1:1, 3:4, 4:3, 9:16, 16:9 — up to 4K on the Identity tier

**Who it is for** — character sheets and storyboards that must stay consistent across frames; product shots with the same model in different outfits; avatars in a chosen style; UGC-style ad creatives without booking a shoot; continuous comic panels with a fixed protagonist.

**Where it falls short** — 4K output is gated behind the Identity tier, so iteration at max quality burns credits. Identity is reference-based, not a trained character model: a hard change of camera angle with few references is still the weak spot.

**Alternatives** — [Photo AI](https://photoai.com) (stronger on photoreal product scenes, more of a studio than a single generator), [Leonardo AI](https://leonardo.ai) (much broader model library, much heavier interface).

→ [Full entry](tools/aigenerate.md) · [Features](https://musepics.com/site/aigenerate/features) · [Pricing](https://musepics.com/site/aigenerate/pricing)

---

## Jev FastEval — 0.3-second diagnostic scores

`Text scoring` · [eval.musepics.com](https://eval.musepics.com)

Ten paste-and-score evaluators that return a dashboard instead of a paragraph. You paste a headline, a resume, a contract or an error log and get a score plus the specific flags in roughly 0.3 seconds — no prompt to write, and the same input produces the same output shape every time.

**The ten evaluators** — headline CTR, ad compliance, meta CTR, JSON errors, cold-email spam risk, review pain points, colour palettes, resume ATS, contract risk, ask-anything.

**What it does well**
- Renders a scoring dashboard in ~0.3s instead of streaming prose for 10–15 seconds
- Zero prompt engineering — paste text or drop a PDF
- Stable output: a score, highlighted flags, and the one factor that decided it
- Free tier is genuinely usable: 10 runs/day, no credit card

**Who it is for** — a pre-flight check on ad copy before it goes to a client; resume tailoring against one specific job description; first-pass contract review before a lawyer sees it; tuning titles and meta descriptions; triaging a stack trace or malformed JSON; mining 5–100 buyer reviews for the complaint that repeats.

**Where it falls short** — a score is an opinion with a number on it. The contract scanner is **not legal advice**, and the fixed output shape that makes it fast is also what makes it rigid: for open-ended judgment, a chat model is still the better tool.

**Alternatives** — [ChatGPT](https://chatgpt.com) (more flexible, but you write the prompt and reformat the output every run), [Claude](https://claude.ai) (excellent at long documents, still prose-out rather than score-out).

→ [Full entry](tools/jev-fasteval.md) · [Features](https://musepics.com/site/jev-fasteval/features) · [Pricing](https://musepics.com/site/jev-fasteval/pricing)

---

## Musebrain — a private AI over your own documents

`Personal AI & knowledge` · [ai.musepics.com](https://ai.musepics.com)

Turns your own documents into a private index that answers with citations, instead of pasting context into a chat box every morning. Covers the four things that actually decide whether a personal AI is worth keeping — privacy, memory, ingestion, latency — and compares the main apps without vendor copy.

**What it does well**
- Documents stay in your namespace; no training on your data
- Every answer cites the passage in your own file, so you can check it
- Deleting a document takes its vectors with it — deletion means deletion
- Ingests PDF, DOCX, Markdown and CSV as they are
- Independent comparisons plus a published how-we-test page

**Who it is for** — asking your own research notes a question months later; recalling what you agreed with a client, source email attached; turning a pile of PDFs into something you can interrogate; keeping a private decision log that stays searchable.

**Where it falls short** — it is a guide *and* a workspace, not a replacement for the notes app you already live in. If your notes are already in Notion, the switching cost is real; if they are scattered PDFs, that is exactly the case it solves.

**Alternatives** — [NotebookLM](https://notebooklm.google.com) (free and citation-first, but tied to a Google account and not a permanent personal index), [Notion AI](https://www.notion.com/product/ai) (best if your notes already live in Notion, weaker at ingesting outside PDFs).

→ [Full entry](tools/musebrain.md) · [Features](https://musepics.com/site/musebrain/features) · [Pricing](https://musepics.com/site/musebrain/pricing)

---

## LessonCraft — lesson plans, quizzes and feedback in about ten seconds

`Education` · [teacher.musepics.com](https://teacher.musepics.com)

Three tools that eat the paperwork around teaching: standards-aligned lesson plans with a timed sequence and differentiation, quizzes with the answer key on its own page, and rubric-based feedback that quotes the student's own words.

**What it does well**
- Lesson plans cite the anchor standard and include objectives, a timed sequence, differentiation, materials and an exit ticket
- Quizzes in four formats — multiple choice, short answer, true/false, fill-in-the-blank — with a separate answer key
- Feedback quotes the student's own work, names what worked, and says exactly what to fix next
- Aligns to Common Core, NGSS, TEKS, Florida BEST, UK, Australian, IB or AP
- Student responses are graded and discarded — not stored, not trained on
- Exports to .docx, prints letter-size, or copies as Markdown for Google Docs and your LMS

**Who it is for** — weekly planning without a blank page; building a quiz and answer key in one sitting; rubric feedback at class scale instead of essay scale; emergency sub plans that still cite a standard.

**Where it falls short** — the free tier has a monthly cap, and "standards-aligned" means the framework is respected, not that your specific district's pacing guide is. Budget a read-through before it reaches a classroom.

**Pricing** — free to start, no credit card. $12/month or $84/year if the free cap gets in the way.

**Alternatives** — [MagicSchool](https://www.magicschool.ai) (the widest catalogue of teacher prompts, breadth over depth), [Brisk Teaching](https://www.briskteaching.com) (browser extension, works inside existing docs and LMS pages).

→ [Full entry](tools/lessoncraft.md) · [Features](https://musepics.com/site/teacher-ai/features) · [Pricing](https://musepics.com/site/teacher-ai/pricing)

---

## How this list is built

Three rules that keep it short and the recommendations usable. The long version is in [guides/how-we-test.md](guides/how-we-test.md).

**01 — Every listing is visited.** A tool only appears here after we have opened it, run the main flow, and read the pricing page. No entry is written from a press release or a landing page.

**02 — No paid placement.** Ordering is editorial. If a tool is listed because it is ours, the entry says so. Nothing is promoted for money, and nothing is buried because a competitor asked.

**03 — Short beats complete.** One strong entry per job beats fifty mediocre ones you have to sift. When a better tool shows up, the weaker one gets removed instead of appended.

---

## Disclosure

These four tools are built by the same team that maintains this list. That is stated in every entry, not buried in a footer — a directory with four entries and no disclosure is just an ad.

The comparison pages link to real competitors ([Photo AI](https://photoai.com), [Leonardo AI](https://leonardo.ai), [ChatGPT](https://chatgpt.com), [Claude](https://claude.ai), [NotebookLM](https://notebooklm.google.com), [Notion AI](https://www.notion.com/product/ai), [MagicSchool](https://www.magicschool.ai), [Brisk Teaching](https://www.briskteaching.com)) because a list where the only answer is "us" is worthless to you.

---

## Contributing

Found a tool that does one job better than the entry here? Open an issue with: what it does, the free tier, and one thing it is bad at. Entries without a stated weakness do not get merged. See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

[CC0 1.0](LICENSE) — copy, fork, translate, republish. A link back is appreciated, not required.

---

<sub>Maintained alongside [MusePics Directory](https://musepics.com/) · 目录由 [木薯派](https://musepics.com/) 维护 · 有 AI，薯你最派</sub>

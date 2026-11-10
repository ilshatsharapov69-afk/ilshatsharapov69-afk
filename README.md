# Ilshat Sharapov · AI automation engineer

I bring AI into how a business actually works: AI agents and LLM assistants, RAG over a company's own
material, Telegram bots and Mini Apps, scrapers, and integrations between the tools a team already uses.

I build with Claude Code in a fixed order: a plan and a spec, the agent writes the code, automated tests,
an independent review in a fresh session, then my own acceptance. Before AI I worked in industrial
automation and power engineering (automation cabinets, controllers, commissioning), so I start from the
process, not from the model.

## What I have built

- **AI sales assistant on the Claude API.** Answers site visitors in a chat and by email, stores every
  conversation in a database, and pings the owner in Telegram, who can take over. About 3 cents of API
  cost per answer, measured on the live setup.
- **Shared inbox as a Telegram Mini App.** Messages from a site chat, email, a contact form and YouTube
  comments land in one list: reply, snooze, add notes, or take the conversation over from the AI.
- **Lead-qualification bot + sales-team Mini App.** A Telegram bot on Cloudflare Workers hands each lead to
  a consultant; a Mini App lets the team filter leads, set statuses and owners, and read funnel stats.
- **RAG knowledge base over Telegram channels.** Downloads channels, transcribes voice and video locally
  with faster-whisper on a GPU, indexes the chunks with embeddings in LanceDB, and answers through Claude
  with a link to the exact source and timestamp.
- **YouTube research scraper and analyzer.** My own replacement for a paid niche-research tool: reads
  public comment and transcript endpoints with no API key into SQLite, with filterable dashboards.

These run on private code. I am glad to walk through any of them on a screen share.

## Live demos you can try

| Demo | What it shows |
|---|---|
| [AI inbox agent](https://ai-inbox-agent-demo.sherlock753cc.workers.dev/) | An LLM sorts incoming requests and drafts a reply to each |
| [RAG knowledge base](https://rag-knowledge-base-demo.sherlock753cc.workers.dev/) | Answers over a fictional company's documents, vector + full-text search, with citations |
| [Print shop sales bot](https://print-shop-bot-demo.sherlock753cc.workers.dev/) | A chat bot that quotes an order and hands it to the owner (fictional shop) |
| [Telegram FAQ and booking bot](https://t.me/shov_demo_bot) | FAQ answers, booking, and a lead card for the owner, in English and Russian |
| [Telegram Mini App CRM](https://tg-crm-miniapp-demo.sherlock753cc.workers.dev/) | A sales team's lead list, statuses and funnel, in a browser sandbox |
| [Landing page + cost quiz](https://landing-quiz-demo.sherlock753cc.workers.dev/) | A 5-step quiz that gives an estimate and sends the lead to a database and Telegram |
| [Price monitor](https://price-monitor-demo.sherlock753cc.workers.dev/) | A scraper with a dashboard of price changes on a Worker + D1 |
| [YouTube packaging tool](https://video-packager-demo.sherlock753cc.workers.dev/) | Titles, chapters, tags and thumbnail text for a video; an outlier finder |

The web demos run on Cloudflare Workers with D1 and Workers AI; the AI ones have per-visitor limits.

## Public code here

- [whisper-typing](https://github.com/ilshatsharapov69-afk/whisper-typing): voice typing for Windows. An
  open-source fork I extended (tray, overlay, media auto-pause, hold-to-record, history, self-recovery).
- [crm-data-extractor](https://github.com/ilshatsharapov69-afk/crm-data-extractor): Playwright logs into a
  web CRM, flattens nested records and writes them to Google Sheets on a schedule.
- [web-scraping-portfolio](https://github.com/ilshatsharapov69-afk/web-scraping-portfolio): three Python
  scrapers (API, browser automation, directory leads with scoring).
- [living-ledger](https://github.com/ilshatsharapov69-afk/living-ledger): a scroll-driven Astro site, a
  design demo for a small accounting firm.

## Stack

Python · TypeScript / JavaScript · Claude API · Cloudflare Workers, D1, Pages, Workers AI, Vectorize ·
grammY · aiogram · FastAPI · Playwright · SQLite · LanceDB · faster-whisper · Astro · GitHub Actions.
n8n, Make or Zapier when the team already uses them.

## Contact

Telegram [@shov69](https://t.me/shov69) · [sherlock753cc@gmail.com](mailto:sherlock753cc@gmail.com) ·
portfolio [setpointaudit.com](https://setpointaudit.com/)

Open to remote roles in AI automation and AI implementation.

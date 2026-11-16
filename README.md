# YouTube Research Skill

One skill for finding what will work on YouTube before a single word is
written — verify the facts, rank the topics, score the hook, package title
+ thumbnail as one pairing, and plan the first-48h push. No API key needed
for the core work: it runs on transcripts and public data.

## What is in here

| Path | What it is |
|---|---|
| `SKILL.md` | **The unified skill — start here.** Research discipline, topic finding, hook scoring, packaging, retention, first-48h push. |
| `skills/claude-youtube/` | 14 YouTube creator sub-skills — audit, seo, script, hook, thumbnail, strategy, calendar, shorts, analyze, repurpose, monetize, competitor, metadata, ideate (MIT, Daniel Agrici). |
| `skills/youtube-agent-skill/` | 11 free YouTube sub-skills — yt-script, yt-package, yt-viral, yt-retention, yt-shorts, yt-edit, yt-seo, yt-chapters, yt-comment, yt-plan, yt-audit (MIT, Jake Schincariol). |
| `docs/research-methods.md` | How to rank a viral topic, spot a niche or pattern, and audit a competitor — the method, not just the tools. |
| `NOTICE.md` | Attribution for every vendored component — read it before reusing anything. |

## Quick start

```bash
git clone https://github.com/<you>/youtube-research-skill.git
cd youtube-research-skill
```

No installs, no keys. Read `SKILL.md`, then route: `yt-viral` for what is
moving now, `yt-script` for hook scoring, `yt-package` for title +
thumbnail, `yt-retention` after publish.

## The research in one paragraph

Verify every fact from primary sources and keep a "do not say" list. Rank
topics by views velocity, not lifetime views, and look for the formula
behind the winner. Score the hook before you waste a take. Lock title +
thumbnail as one pairing a day before publish and check it at 120px. After
publish, read retention to the exact second people left, reply to every
comment in the first 2 hours, and check CTR at hour 4–6 — swap the
thumbnail only if CTR is under ~3%.

## What it does NOT do

- **No editing, narration or production.** That is the companion skill —
  see `video-editing-skill`.
- **No YouTube API by default.** The skills work from transcripts and
  public data; live API use is optional and needs a key.
- **No magic.** The skill measures and reports; it does not decide what is
  good. A topic is real when its sources check out and its velocity is
  measured — not before.
- **No re-licensing of other people's work.** Every vendored component keeps
  its original licence and attribution — see `NOTICE.md`. Only our own
  original work is MIT under this repo's `LICENSE`.

## Honesty rule

Never call research complete unless the sources are cited and the weak
claims are flagged. Report measured numbers, not adjectives.

## Licence

Our original work (the unified skill, the research-methods doc, this README)
is MIT — see `LICENSE`. Vendored components keep their own licences — see
`NOTICE.md` and each `skills/*/VENDORED.md`.

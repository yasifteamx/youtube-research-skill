---
name: youtube-research-skill
description: Research a YouTube topic, niche or competitor before a single word is written — verify the facts, score the hook, package title + thumbnail as one pairing, and plan the first-48h push. Use when the user asks for video ideas, viral topics, a niche or pattern, competitor analysis, a title/thumbnail, SEO, retention analysis or a Shorts plan. No API key needed for the core work — it runs on transcripts and public data.
---

# YouTube Research Skill — one skill for finding what will work

This skill finds the video before it is made: the topic, the angle, the hook
and the package. It is the single entry point; the vendored skills in
`skills/` do the specialist work. Route to them, don't re-implement them.

## The research discipline

1. **Verify every fact from primary sources** (court records, police
   statements, verified reporting) before it enters a script. Never claim a
   solve, arrest or conviction that did not happen. Never invent motive,
   dialogue or a first-person voice for a deceased person. Keep a "do not
   say" list per case or topic.
2. **Demand is earned, not assumed.** A topic wins when it is fresh, has a
   genuine twist, or fills a gap a big channel left open. A stale compilation
   of old news loses — check the trend first (see `docs/research-methods.md`).
3. **Record the source for every claim** you pass on — link or outlet + date.
   If a claim traces to a single thin source, flag it, don't launder it.
4. **Bring patterns, not just topics.** A title formula that works across
   videos, a sub-pattern (e.g. suspects arrested decades later), a format
   gap — these are worth more than one more topic list.

## Find the topic

- **Viral topics** — rank by views velocity (views in the first days), not
  lifetime views. A video doing 100K in 3 days beats a 2M video from 2021.
  Look for the formula behind the winner: the exact title shape, the
  reveal structure, the first-30-seconds promise.
  → `skills/youtube-agent-skill/skills/yt-viral`,
  `skills/claude-youtube/sub-skills/competitor.md` + `analyze.md`.
- **Niches & patterns** — scan adjacent channels for formats nobody in the
  niche is doing yet (on-camera host, explainer series, regional cases,
  Shorts-to-long funnel). Log every find with why it could work and what it
  would need. See `docs/research-methods.md`.
- **Competitors** — audit a channel: upload cadence, view distribution
  (which 20% of videos drive 80% of views), title/thumbnail patterns,
  comment sentiment (what viewers keep asking for is the next video).
  → `skills/claude-youtube/sub-skills/audit.md`, `competitor.md`,
  `strategy.md`, `skills/youtube-agent-skill/skills/yt-audit`, `yt-plan`.

## Score the hook before you waste a take

- **Hook formulas** — 21 formulas with scoring.
  → `skills/youtube-agent-skill/skills/yt-script`,
  `skills/claude-youtube/sub-skills/hook.md` + `script.md`.
- **Structure that holds:** hook 0:00–0:05 grab, 0:05–0:15 promise,
  0:15–0:30 stakes; no "Hey guys welcome back". Pattern interrupt every
  30–60s, open loops, chapters.
- **Script** — size from measured delivery pace (narration words ÷ finished
  minutes of the last video), never from an assumed words-per-minute.
  Expand a short script with verified material, never padding.

## Package title + thumbnail as one pairing

- **Titles** under 50 chars, hook front-loaded in the first 45 characters.
  Thumbnail ≤5 words, never duplicating the title. Title + thumbnail are
  one pairing — lint them together, not separately.
  → `skills/youtube-agent-skill/skills/yt-package`,
  `skills/claude-youtube/sub-skills/thumbnail.md` + `metadata.md`.
- **CTR is the whole game.** Check the package at 120px (phone size) before
  publish: big face or object, 3–4 words max, one red banner element, high
  contrast. Packaging is locked before publish, not after.
- **SEO** — tags, description, chapters from the finished video, not the
  plan.
  → `skills/youtube-agent-skill/skills/yt-seo`, `yt-chapters`,
  `skills/claude-youtube/sub-skills/seo.md` + `metadata.md`.

## After publish: retention and the first 48 hours

- **Retention** — read the retention export and find the exact second
  people left and what was being said there. That second is the next
  video's fix.
  → `skills/youtube-agent-skill/skills/yt-retention`.
- **Comments** — reply to every comment in the first 2 hours, pin a
  question comment, mine comments for the next topic.
  → `skills/youtube-agent-skill/skills/yt-comment`.
- **First-48h push** — community teaser + Short 24h before publish; CTR
  check at hour 4–6 — swap the thumbnail only if CTR < ~3%; review the
  trajectory at hour 48. Don't judge a video in its first 7 days.
- **Shorts funnel** — 2–3 Shorts per long video: hook in 1–3s, captions on,
  end on the long video.
  → `skills/youtube-agent-skill/skills/yt-shorts`,
  `skills/claude-youtube/sub-skills/shorts.md` + `repurpose.md`.
- **Channel strategy & monetisation** — calendar, monetise, strategy.
  → `skills/claude-youtube/sub-skills/calendar.md`, `monetize.md`,
  `strategy.md`.

## What never works

Never sub4sub, never buy views, never lie in the clickbait. Never present a
rumour as a solve. Never build a video on a single unverified viral claim —
if the only source is a site that fabricates "solved" stories, drop the
topic and say why.

## Honesty rule

Never call research complete unless the sources are cited and the weak
claims are flagged. Report measured numbers (views, velocity, CTR), not
adjectives, and disclose what you could not verify before the user builds
on it.

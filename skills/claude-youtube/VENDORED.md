# Vendored: claude-youtube

- **Source:** https://github.com/AgriciDaniel/claude-youtube — by Daniel Agrici.
- **Licence:** MIT — Copyright (c) 2025 Daniel Agrici. Original `LICENSE` file kept in this folder.
- **What it is:** a YouTube creator skill with 14 sub-skills (audit, seo, script, hook, thumbnail, strategy, calendar, shorts, analyze, repurpose, monetize, competitor, metadata, ideate) plus execution scripts (`execution/fetch_channel_data.py`, `fetch_transcript.py`, `fetch_video_analytics.py`, `search_competitor_videos.py`). The main `SKILL.md` is the command router.
- **Kept/changed:** vendored unchanged (no `.git` was present in the local copy).
- **How we use it in this repo:** hook/script/thumbnail/metadata/competitor routing — see the root `SKILL.md` "YouTube packaging" section. Note: live YouTube API use is optional and needs a key; the skill works from transcripts and public data without one.
